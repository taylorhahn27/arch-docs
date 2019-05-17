<!-- this refers to Johns current drawing, it is complex, it requires a join in javascript
-->

sequenceDiagram
    Apollo GQL Server->>HKS GQL Server: get resourceIDs()
    HKS GQL Server-->>Apollo GQL Server: here are resourceIDs()
    Apollo GQL Server->>HKS GQL Server: get projects()
    HKS GQL Server-->>Apollo GQL Server: here are projects()
    Apollo GQL Server->>HKS GQL Server: get resource-project() join table
    HKS GQL Server-->>Apollo GQL Server: here is the resource-project() join table
    Apollo GQL Server->>Apollo GQL Server: join resources with projects
