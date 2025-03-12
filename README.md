# Santander Dev Week 2023
Java RESTful API criada para a Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        +String name
        +Account account
        +List~Feature~ features
        +Card card
        +List~News~ news
    }

    class Account {
        +String Number
        +String Agency
        +Float Balance
        +Float Limit
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String Number
        +Float Limit
    }

    class News {
        +String icon
        +String description
    }

    User "1" *-- "1" Account
    User "1" *-- "1..N" Feature
    User "1" *-- "1" Card
    User "1" *-- "N" News
```
