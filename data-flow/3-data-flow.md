<!--
Proposed API, join is done in SQL server
--->

sequenceDiagram
    Apollo GQL Server->>HKS GQL Server: get resource details with assignments()
    HKS GQL Server-->>Apollo GQL Server: here are all resource details with their assignments
