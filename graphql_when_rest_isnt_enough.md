---
target: This talk is targeted at developers with existing REST APIs with ballooning complexity or engineers looking at GraphQL as an API solution in Ruby.
---

# GraphQL: When REST isn't enough

## Abstract
Find out why many large-scale production Rails applications are adopting GraphQL

_OR_

REST has been the predominant standard for Rails APIs since it's inception.  But as Ruby matures and more requirements placed on production Rails environments, many engineers are switching to GraphQL and here's why.

## Details
1. What is GraphQL?
2. REST vs. GraphQL
  - REST is:
    - Resource driven
    - Well known and intrinsic in Rails
    - Simpler with lower switching costs
    - Complex for production-scale applications
  - GraphQL is:
    - Client-driven
    - Type system
      - Define-it-and-forget-it
      - Strongly typed
    - Overly complex for small-scale deployments
3. How to implement GraphQL in Rails
  - The `graphql-ruby` gem
    - Existing implementation
    - New class-based implementation
  - Basic setup in a Rails app
  - Strategies for introducing GraphQL to existing REST APIs
4. Conclusions and moving forward

## Pitch
I've implemented several GraphQL APIs using `graphql-ruby` at both AssembledBrands and StackShare.  I've also been heavily involved in the graphql-ruby community helping to develop conventions and processes for production-scale Ruby implementations

## References
1. [The Github GraphQL API](https://githubengineering.com/the-github-graphql-api/)
