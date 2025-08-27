    # Problem 29. 이슈 5개(제목/작성자) 가져오기

    **Endpoint**: GitHub

    ## 🎯 목표
    `issues(first:5, states:OPEN)`의 `title, author{login}`

    ## ▶ 스타터 쿼리
    ```graphql
    query IssuesBasic($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    issues(first: 5, states: OPEN, orderBy:{field:CREATED_AT, direction:DESC}) {
      nodes { title author { login } }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react"}
```
