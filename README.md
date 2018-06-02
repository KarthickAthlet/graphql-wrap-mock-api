# Wrap Your API with GraphQL

## Quick Start


```
npm install
```

Then run these commands in separate terminal windows.
```
npm run start:api-server
npm run start:graphql-server
```

Open http://localhost:5000

## Sample Query

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
