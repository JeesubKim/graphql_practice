    # Problem 43. 최근 1개월 PR/Issue 통계

    **Endpoint**: GitHub

    ## 🎯 목표
    ISO 날짜 문자열 변수를 사용해 `createdAt` 기준 필터.

    ## ▶ 스타터 쿼리
    ```graphql
    query RecentStats($from: DateTime!) {
  viewer {
    repositories(first: 20, orderBy:{field:UPDATED_AT, direction:DESC}) {
      nodes {
        name
        recentPRs: pullRequests(first: 1, orderBy:{field:CREATED_AT, direction:DESC}, after: null, states: OPEN) {
          totalCount
        }
        recentIssues: issues(first: 1, orderBy:{field:CREATED_AT, direction:DESC}, after: null, states: OPEN) {
          totalCount
        }
      }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"from":"2025-07-01T00:00:00Z"}
```
## 💡 힌트/주의
쿼리에서 직접 createdAt 필터가 제한적이라 search API 조합을 고려해도 좋습니다.
