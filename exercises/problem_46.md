    # Problem 46. Pagination + Variables 조합

    **Endpoint**: GitHub

    ## 🎯 목표
    `issues(first:$n, after:$cursor)` 패턴 구현.

    ## ▶ 스타터 쿼리
    ```graphql
    query IssuesScroll($owner: String!, $name: String!, $n: Int!, $cursor: String) {
  repository(owner: $owner, name: $name) {
    issues(first: $n, after: $cursor, states: OPEN, orderBy:{field:CREATED_AT, direction:DESC}) {
      pageInfo { hasNextPage endCursor }
      nodes { number title createdAt author { login } }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react","n":5,"cursor":null}
```
