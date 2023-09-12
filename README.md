# Santander Dev Week 2023 
Java RESTful API criada para o SAntander Dev Week.

## Diagrama de classes

```mermaid
classDiagram
  class Usuario {
    - nome: String
    - account: Conta
    - feature: List<Feature>
    - card: Cartao
    - news: List<Novidade>
  }

  class Conta {
    - number: String
    - agency: String
    - balance: Float
    - limit: Float
  }

  class Feature {
    - icon: String
    - description: String
  }

  class Cartao {
    - number: String
    - limit: Float
  }

  class Novidade {
    - icon: String
    - description: String
  }

  Usuario -- Conta : possui
  Usuario -- Feature : possui
  Usuario -- Cartao : possui
  Usuario -- Novidade : possui

```
