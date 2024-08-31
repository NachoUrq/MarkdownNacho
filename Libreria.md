```mermaid
classDiagram
    class Adulto {
        +String titulo
        +String autores
        +String isbn
        +boolean isAvailable()
    }

    class Niño {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }
 class Familia {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class Vida {
        +String name
        +String employeeId
        +addBook(Book book)
        +removeBook(Book book)
    }



    Adulto --> Familia : dicta
    Niño --> Vida : pertenece a
    clase --> Familia : en
    

    Adulto --> Familia : administra
