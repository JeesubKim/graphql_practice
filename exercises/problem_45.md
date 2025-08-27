    # Problem 45. Variables로 레포 이름 외부 입력

    **Endpoint**: GitHub

    ## 🎯 목표
    `$owner, $name` 변수를 받아 레포 정보를 조회.

    ## ▶ 스타터 쿼리
    ```graphql
    query RepoByVar($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    name description url
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react"}
```
