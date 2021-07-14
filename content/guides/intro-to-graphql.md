# Intro to GraphQL

## GraphQL 101

GraphQL is a query language for your API, and a server-side runtime for executing queries using a type system you define for your data. GraphQL isn't tied to any specific database or storage engine and is instead backed by your existing code and data.

**For more details, please refer to the** [**official GraphQL docs**](https://graphql.org/)**.**

## Schema

A GraphQL service is created by defining types and fields on those types, then providing functions for each field on each type. For example, a GraphQL service that tells you who the logged in user is \(`me`\) as well as that user's name might look like this:

```graphql
type Query {
  me: User
}
 
type User {
  id: ID
  name: String
}
```

## Query

After a GraphQL service is running \(typically at a URL on a web service\), it can receive GraphQL queries to validate and execute. The service first checks a query to ensure it only refers to the types and fields defined, and then runs the provided functions to produce a result.


For example, the query:

```text
{  me {    name  }}
```

Could produce the following JSON result:

```text
{  "me": {    "name": "Luke Skywalker"  }}
```

## IDE

GraphiQL is the GraphQL integrated development environment \(IDE\). It’s a powerful \(and all-around awesome\) tool you’ll use often while building Gatsby websites.

**Whitehead ships with a built-in GraphiQL IDE that you can access from** [**the dashboard itself**](https://dashboard.whitehead.ai)**.**

{% embed url="https://www.gatsbyjs.com/graphiql-explore.mp4" %}

