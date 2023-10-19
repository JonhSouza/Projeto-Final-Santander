# Santander bootcamp 2023
Java RESTful Api para o projeto final

## Diagrama de classes

```mermaid

classDiagram
  class User {
    - name: String
    - account: Account
    - features: Feature[]
    - card: Card
    - news : News[]
  }
  class Account {
    - number: String
    - agency: String
    - balance: number
    - limit: Number
  }
  class Features {
    - icon: String
    - description: String
  }
  class Cards {
    - number: String
    - limit: Number
  }
  class News {
    - icon: String
    - description: String
  }
  User *-- Account
  User *-- Features 
  User *-- Cards
  User *-- News
