#Santander Dev Week 2024

##Diagrama de Classes

```mermaid
classDiagram
    class User {
        -String name
        -Account account
        -Card card
        -List~Feature~ features
        -List~News~ news
    }

    class Account {
        -String number
        -String agency
        -double balance
        -double limit
    }

    class Feature {
        -String icom
        -String descripition
    }

    class Card {
        -String number
        -double limit
    }

    class News {
        -String icom
        -String descripition
    }

    User "1" * --"1" Account
    User "1" * --"1" Card
    User "1"  *-- "N"Feature
    User "1"  *--"N" News 
```
