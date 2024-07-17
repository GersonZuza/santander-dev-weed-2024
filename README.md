# Santander Dev Week 2024
Java RESTful API criada para o Santander Dev Week.

## Diagrama de Classes

```mermaid
classDiagram
    class User {
        - name: string
        - account: Account
        - features: Feature[]
        - card: Card
        - news: News[]
    }

    class Account {
        - number: string
        - agency: string
        - balance: float
        - limit: float
    }

    class Card {
        - number: string
        - limit: float
    }

    class Feature {
        - icon: string
        - description: string
    }

    class News {
        - icon: string
        - description: string
    }

    User --> Account
    User --> Card
    User --> Feature
    User --> News
```
