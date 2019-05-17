<!-- Apollo Current
-->

sequenceDiagram
    Apollo Client->>Apollo Server: Get all thumbnails()
    Apollo Server-->>Apollo Client: Here are all thumbnails
    Apollo Client->>Apollo Server: Get all Project Details(ResourceID)
    Apollo Server-->>Apollo Client: Here are all Project Details
    Apollo Client->>Apollo Server: Get all Current Projects()
    Apollo Server-->>Apollo Client: Here are all Current Projects

