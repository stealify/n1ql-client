# n1ql-client
This is the Couchbase N1QL Query Client working in Node and the Browser

```
import n1ql from n1ql-client
// Handels Reconnect Scenarios and Bindings
n1ql
  .connect('https://cluster.url')
  .auth('user', 'token') // Create and Manage users via n1ql-interface
  
const query = n1ql.query;
// All querys get executed with the permissions of the user
// You can Manage that Permissions via n1ql-interface or programatic via server side n1ql-client **Link Documentation**
query('SELECT * from default').then(data=>console.log,err=>console.error);
```

## UpComing integrations
GraphQL -> n1ql
n1ql -> GraphQL

## Guides
- Build N1QL driven api endpoints with user authencication and Access Permissions
- Build GraphQL driven api endpoints including user authencication and Access Permissions porting all N1QL Features to GraphQL

## References
- Additional Couchbase RBAC
