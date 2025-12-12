
### B) `diagrams/sequence-login.md`
```md
```mermaid
sequenceDiagram
  actor U as User
  participant B as Browser
  participant S as Flask Server
  participant F as users.json

  U->>B: Enter email & password
  B->>S: POST /login
  S->>F: load_users()
  F-->>S: users list
  alt valid credentials
    S-->>B: Redirect /dashboard
    B->>S: GET /dashboard
    S-->>B: dashboard.html
  else invalid
    S-->>B: Redirect /
  end
