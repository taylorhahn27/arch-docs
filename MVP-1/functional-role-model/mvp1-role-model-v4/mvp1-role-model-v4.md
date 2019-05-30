```mermaid
graph BT;
a(HKS SQL Data Warehouse) --> b(SQL Server);
subgraph Current -- HKS
b --> c(Apollo<br>Client/Server);
c --> d(on Azure);
end
subgraph Role Models
a --> e(Relational Database);
e --> f(GQL Client/Server);
f --> g(Serverless);
end
a --> h(Postgres);
subgraph Relatable Partners
h --> i;
i(Apollo<br>Client/Server) --> j(Zeit);
end
```