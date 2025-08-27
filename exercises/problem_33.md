    # Problem 33. Fork 만들기 (CreateFork)

    **Endpoint**: GitHub

    ## 🎯 목표
    `createFork(input:{ repositoryId:$id })`

    ## ▶ 스타터 쿼리
    ```graphql
    mutation Fork($id: ID!) {
  createFork(input: { repositoryId: $id }) {
    repository { id name owner { login } }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"id":"<REPO_RELAY_ID>"}
```
