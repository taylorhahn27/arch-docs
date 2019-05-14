```mermaid
graph BT;
    A(HKS SQL D.W.)-->B(Postgres);
    A-->C(SQL Server);
    B-->D(Apollo<br> Client/Server);
    C-->E(Apollo<br> Client/Server);
    D-->F(Zeit);
    E-->G(On Azure);
```