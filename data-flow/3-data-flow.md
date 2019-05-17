<!--
Proposed API, join is done in SQL server
--->
```mermaid
sequenceDiagram
    Apollo GQL Server->>HKS GQL Server: get resource details with assignments()
    HKS GQL Server-->>Apollo GQL Server: here are resource details with their assignments
```