    # Problem 35. 이슈 닫기

    **Endpoint**: GitHub

    ## 🎯 목표
    `closeIssue(input:{ issueId })`

    ## ▶ 스타터 쿼리
    ```graphql
    mutation CloseIssue($issueId: ID!) {
  closeIssue(input: { issueId: $issueId }) {
    issue { number state }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"issueId":"<ISSUE_ID>"}
```
