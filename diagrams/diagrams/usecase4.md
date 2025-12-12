
### D) `diagrams/deployment.md`
```md
```mermaid
flowchart TB
  U[User Browser] -->|HTTP| APP[Flask App]
  APP -->|reads/writes| JS[(users.json)]
