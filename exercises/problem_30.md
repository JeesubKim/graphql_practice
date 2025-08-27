    # Problem 30. PR 5개 pagination

    **Endpoint**: GitHub

    ## 🎯 목표
    `pullRequests(first:$n, after:$c)`와 `pageInfo`

    ## ▶ 스타터 쿼리
    ```graphql
    query PRsPage($owner: String!, $name: String!, $n: Int!, $c: String) {
  repository(owner: $owner, name: $name) {
    pullRequests(first: $n, after: $c, orderBy:{field:CREATED_AT, direction:DESC}) {
      pageInfo { hasNextPage endCursor }
      nodes { title number createdAt author { login } }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react","n":5,"c":null}
```
