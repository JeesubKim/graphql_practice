    # Problem 34. 이슈 생성

    **Endpoint**: GitHub

    ## 🎯 목표
    `createIssue(input:{ repositoryId, title, body })`

    ## ▶ 스타터 쿼리
    ```graphql
    mutation CreateIssue($input: CreateIssueInput!) {
  createIssue(input: $input) {
    issue { number title url author { login } }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"input":{"repositoryId":"<REPO_ID>","title":"Hello","body":"From GraphQL"}}
```
