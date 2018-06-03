# Wrap Your API with GraphQL

## What's this about?

This project shows how to wrap an existing REST API with GraphQL. 

## How's this work?

1. This project contains an API created via [json-server](https://github.com/typicode/json-server). It serves fake data generated via [faker.js](https://github.com/Marak/faker.js).
2. The REST API is wrapped with GraphQL, which is hosted via [Express](https://expressjs.com). GraphQL is integrated with Express via [express-graphql](https://github.com/graphql/express-graphql) middleware.
3. The express-graphql middleware includes [GraphiQL](https://github.com/graphql/graphiql), a web-based tool for running GraphQL queries. We'll use this to run GraphQL queries.

## Quick Start

1) Install dependencies.
```
npm install
```

2) Run these commands in separate terminal windows.
```
npm run start:api-server
npm run start:graphql-server
```

3) Open http://localhost:5000

## Sample Query

Run this in GraphiQL.

```
{
  posts(page: "2") {
    title
    author {
      lastName
      company {
        companyDescription
      }
    }
  }
}
```

---

## Credit

This demo is inspired by [Eric Baer's GraphQL For The Rest of Us](https://github.com/baer/graphql-demo-graphql-for-the-rest-of-us).
