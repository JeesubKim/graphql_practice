    # Problem 32. Star 제거 (RemoveStar)

    **Endpoint**: GitHub

    ## 🎯 목표
    `removeStar(input:{starrableId:$id})`를 실행하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    mutation RemoveStar($id: ID!) {
  removeStar(input: { starrableId: $id }) {
    starrable { id viewerHasStarred stargazerCount }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"id":"<REPO_ORG_RELAY_ID>"}
```
