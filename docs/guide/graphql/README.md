# GraphQL Schema

This plugin has an opinion of how the GraphQL API schema should look like:

- Query for multiple records is plural camelCase: `blogPosts`
- Mutations begin with the verb (`create`, `update`, `delete`) and the camelCased entity: `createBlogPost` for example.
- The create mutation expects the new record as a input type argument
- The update mutation expects two arguments: The ID and the new record as a input type
- The delete mutation expects the record ID to delete
- Multiple records are within a `nodes` object and filtered by a `filter` argument.