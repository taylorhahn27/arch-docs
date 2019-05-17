<!-- Apollo Current
-->

sequenceDiagram
    Apollo Client->>Apollo Server: get thumbnails()
    Apollo Server-->>Apollo Client: here are thumbnails
    Apollo Client->>Apollo Server: get project details(ResourceID)
    Apollo Server-->>Apollo Client: here are project details
    Apollo Client->>Apollo Server: get current projects()
    Apollo Server-->>Apollo Client: here are current projects

