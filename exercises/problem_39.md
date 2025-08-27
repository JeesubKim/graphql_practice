    # Problem 39. 브랜치 리스트

    **Endpoint**: GitHub

    ## 🎯 목표
    `refs(refPrefix:"refs/heads/", first:10)`에서 `name, target.oid`

    ## ▶ 스타터 쿼리
    ```graphql
    query Branches($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    refs(refPrefix: "refs/heads/", first: 10) {
      nodes { name target { oid } }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react"}
```
