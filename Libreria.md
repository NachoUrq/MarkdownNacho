```mermaid
classDiagram
    class adulto {
        +String titulo
        +String autores
        +String isbn
        +boolean isAvailable()
    }

    class nino {
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
    nino --> vida : pertenece a
    clase --> familia : en
    

    adulto --> familia : administra
