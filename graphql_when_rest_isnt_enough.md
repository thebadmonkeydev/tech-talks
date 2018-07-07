---
target: This talk is targeted at developers with existing REST APIs with ballooning complexity or engineers looking at GraphQL as an API solution in Ruby.
bio: Michael Kelly, Senior Backend Engineer at StackShare, is passionate about two things, Ruby APIs and building motorcycles.  He’s been building with Rails in and around the startup world for more than eight years and has been focused on GraphQL as a technology for the last two.  He tweets a little and is generally just a bad monkey.
---

# GraphQL: When REST isn't enough

## Abstract
REST has been the predominant standard for Rails APIs since it's inception.  But as Ruby matures and more requirements placed on production Rails environments, many large APIs such as Github, Shopify, Intuit, and Drupal are switching to GraphQL and here's why.

## Details
I've developed Ruby GraphQL APIs in production for the last two years and have worked directly on the growth and adoption of the `graphql-ruby` gem.  I love GraphQL!  In this talk I'm going to address the differences between REST and GraphQL as they manifest in a modern Rails application along with strategies for adopting GraphQL incrementally in existing REST applications.
I will also be covering.

1. When REST isn't enough
  - Incomplete data sets
  - Multiple network requests for full data context
  - All the data all the time (full objects)
2. Enter GraphQL
  - What it is
  - Where it came from
    - Rapid client development
    - API evolution
3. GraphQL vs. REST
  - REST is:
    - Well known and intrinsic in Rails
    - Simpler with lower switching costs
    - Complex for production-scale applications
    - Ad-hoc and often internally motivated abstraction
  - GraphQL is:
    - Client-driven
    - Type system
      - Define-it-and-forget-it
      - Strongly typed
      - Clean layer of abstraction
    - Overly complex for small-scale deployments
3. Should you adopt GraphQL?
  - They have more than one client application
  - A mobile client/focus on latency and bandwidth
  - Entrenched REST API with ballooning complexity
  - Decouple FE and BE development
  - Business perspective
4. GraphQL the Rails Way
  - The `graphql-ruby` gem
    - Existing implementation
    - New class-based implementation
  - Basic setup in a Rails app
  - Strategies for introducing GraphQL to existing REST APIs
5. Conclusions and moving forward
  - Community
  - Adoption Strategies
    - Real world example from StackShare's feed

======================================================================
I've developed Ruby GraphQL APIs in production for the last two years and have worked directly on the growth and adoption of the `graphql-ruby` gem.  I love GraphQL!  In this talk I'm going to address the differences between REST and GraphQL as they manifest in a modern Rails application along with strategies for adopting GraphQL incrementally in existing REST applications.  The outline for this presentation is:

1. When REST isn't enough
  - A discussion on the limitations of REST APIs
  - The evolution to client-driven APIs
    - RESTful ways of solving these problems (complex!)
2. Enter GraphQL
  - What is it anyway?
  - Solving the limitations of REST
3. Should you start adopting GraphQL?
  - Examples of problems solved by GraphQL
  - Benefits outside of API design
  - Where GraphQL falls short
4. Doing GraphQL the "Rails Way"
  - The `graphql-ruby` gem
  - The new class-based implementation
  - Basic setup in a **Real** Rails application with example code from StackShare's implementation
  - Strategies for introducing GraphQL in an existing REST-based application
5. Conclusions/Wrap-up
======================================================================


## Pitch
I've implemented several GraphQL APIs using `graphql-ruby` at both AssembledBrands and StackShare.  I've also been heavily involved in the graphql-ruby community helping to develop conventions and processes for production-scale Ruby implementations

## References
1. [The Github GraphQL API](https://githubengineering.com/the-github-graphql-api/)
2. [The Business case for GraphQL](https://dev-blog.apollodata.com/the-business-case-for-graphql-cc7a2b93148d)
