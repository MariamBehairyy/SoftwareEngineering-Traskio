
### C) `diagrams/class-diagram.md`
```md
```mermaid
classDiagram
  class User {
    +email: string
    +password_hash: string
  }

  class FlaskApp {
    +signup()
    +login()
    +dashboard()
    +logout()
    +me()
    +load_users()
    +save_users()
  }

  FlaskApp --> User : reads/writes
