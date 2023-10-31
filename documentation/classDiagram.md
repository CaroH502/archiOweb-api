```mermaid
---
title: Diagramme de classe
---
classDiagram
    User "1" --> "*" Garden : has
    Garden "1" --> "1" User : belongs to
    Garden "1" --> "*" Plant :has 
    Plant "1" --> "1" Garden : belongs to
    class User {
        +idUser
        +username
        +password
        +name
        +surname
        +birthDate
        +createAt
        +modifiedAt
        +create()
        +set()
        +delete()
        +get()
        +checkPassword()
    }
    class Garden {
        +idGarden
        +gardenName
        +localisation
        +fkUser
        +createAt
        +modifiedAt
        +create()
        +delete()
        +get()
        +set()
        +getPlantList()
        +setLocalisation()
    }
    class Plant {
        +latinName
        +family
        +familyNameList
        +description
        +origin
        +exposition
        +maintenance
        +groundType
        +color
        +height
        +bloom
        +plantationDate
        +healthState
        +imgURL
        +useType
        +createAt
        +modifiedAt
        +fkGarden
        +create()
        +set()
        +get()
        +delete()
    }
```
