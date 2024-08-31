```mermaid
classDiagram
    class adulto {
        +String titulo
        +String autores
        +String isbn
        +boolean isAvailable()
    }

    class niño {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }
 class familia {
        +String name
        +String memberId
        +borrowBook(Book book)
        +returnBook(Book book)
    }

    class vida {
        +String name
        +String employeeId
        +addBook(Book book)
        +removeBook(Book book)
    }



    adulto --> familia : dicta
    niño --> vida : pertenece a
    clase --> familia : en
    

    adulto --> familia : administra
