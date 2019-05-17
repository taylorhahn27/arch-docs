<title>Data Flow</title>

## 1. Apollo Current

```mermaid
sequenceDiagram
    Apollo Client->>Apollo Server: Get all thumbnails()
    Apollo Server-->>Apollo Client: Here are all thumbnails
    Apollo Client->>Apollo Server: Get all Project Details(ResourceID)
    Apollo Server-->>Apollo Client: Here are all Project Details
    Apollo Client->>Apollo Server: Get all Current Projects()
    Apollo Server-->>Apollo Client: Here are all Current Projects
```

## 2. In Reference to Johns Current Drawing
* it is complex
* it requires a join in Javascript

```mermaid
sequenceDiagram
    Apollo GQL Server->>HKS GQL Server: get all resourceIDs()
    HKS GQL Server-->>Apollo GQL Server: here are all resourceIDs()
    Apollo GQL Server->>HKS GQL Server: get all projects()
    HKS GQL Server-->>Apollo GQL Server: here are all projects()
    Apollo GQL Server->>HKS GQL Server: get resource-project() join table
    HKS GQL Server-->>Apollo GQL Server: here is the resource-project() join table
    Apollo GQL Server->>Apollo GQL Server: join resources with projects
```

## 3. Proposed API
* join is done in SQL server

```mermaid
sequenceDiagram
    Apollo GQL Server->>HKS GQL Server: get resource details with assignments()
    HKS GQL Server-->>Apollo GQL Server: here are all resource details with their assignments
```