    # Problem 40. 브랜치 마지막 커밋

    **Endpoint**: GitHub

    ## 🎯 목표
    `ref(qualifiedName:"main") { target { ... on Commit { history(first:1){ nodes{ messageHeadline committedDate } } } } }`

    ## ▶ 스타터 쿼리
    ```graphql
    query LastCommit($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    ref(qualifiedName: "main") {
      target {
        ... on Commit {
          history(first: 1) {
            nodes { messageHeadline committedDate }
          }
        }
      }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react"}
```
