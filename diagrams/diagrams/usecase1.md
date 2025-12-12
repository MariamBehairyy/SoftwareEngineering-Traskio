```mermaid
flowchart LR
  Guest([Guest]) --> UC1((Sign Up))
  Guest([Guest]) --> UC2((Log In))
  User([User]) --> UC3((View Dashboard))
  User([User]) --> UC4((Log Out))
  UC3 --> P1[[Requires Session]]
