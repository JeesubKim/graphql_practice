    # Problem 31. Star 추가 (AddStar)

    **Endpoint**: GitHub

    ## 🎯 목표
    `addStar(input:{starrableId:$id})` mutation을 실행하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    mutation AddStar($id: ID!) {
  addStar(input: { starrableId: $id }) {
    starrable { id viewerHasStarred stargazerCount }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"id":"<REPO_ORG_RELAY_ID>"}
```
## 💡 힌트/주의
레포의 글로벌 `id`는 `repository(owner,name){ id }`로 먼저 조회하세요.
