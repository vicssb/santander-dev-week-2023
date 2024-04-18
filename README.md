# Santander Dev Week 2023

##Class Diagram
```mermaid
classDiagram
    class User {
        -String name
        -Account account
        -Feature[] features
        -Card card
        -News[] news
    }
    class Account {
        -String accountNumber
        -String accountAgency
        -Float accountBalance
        -Float accountLimit
    }
    class Feature {
        -String icon
        -String description
    }
    class Card {
        -String number
        -Float limit
    }
    class News {
        -String icon
        -String description
    }
    User "1" *-- "1" Account
    User "1" *-- "N" Feature
    User "1" *-- "1" Card
    User "1" *-- "N" News
```
