# GraphQLCasts
Completed Code Examples from GraphQL with React

npm install

npm run dev

npm run json:server

```
{
  user(id: "40") {
    id
    firstName
    age
  }
}

{
  user(id: "40") {
    id
    firstName
    age
    company {
      id
      name
      description
    }
  }
}


{
  apple: company(id: "1") {
    id
    name
    description
  }
  google: company(id: "2") {
    id
    name
    description
  }
}


{
  apple: company(id: "1") {
    ...companyDetails
  }
  google: company(id: "2") {
    ...companyDetails
  }
}

fragment companyDetails on Company {
  id
  name
  description
}
```
