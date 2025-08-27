    # Problem 47. README 파일 내용 가져오기

    **Endpoint**: GitHub

    ## 🎯 목표
    `object(expression:"main:README.md") { ... on Blob { text } }`

    ## ▶ 스타터 쿼리
    ```graphql
    query Readme($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    object(expression: "main:README.md") {
      ... on Blob { text }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react"}
```
