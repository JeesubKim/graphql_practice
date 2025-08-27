    # Problem 41. 레포에서 PR과 Issue 함께 조회 (inline fragments)

    **Endpoint**: GitHub

    ## 🎯 목표
    `repository { issues(first:3) { nodes{ __typename number title } } pullRequests(first:3){ nodes{ __typename number title } } }`

    ## ▶ 스타터 쿼리
    ```graphql
    query IssuesAndPRs($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    issues(first: 3, orderBy:{field:CREATED_AT, direction:DESC}) {
      nodes { __typename number title author { login } }
    }
    pullRequests(first: 3, orderBy:{field:CREATED_AT, direction:DESC}) {
      nodes { __typename number title author { login } }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react"}
```
