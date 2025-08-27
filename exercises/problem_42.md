    # Problem 42. 내 모든 레포의 Open/Closed 이슈 개수

    **Endpoint**: GitHub

    ## 🎯 목표
    `viewer { repositories(first:100){ nodes{ name issues(states:OPEN){totalCount} issuesClosed:issues(states:CLOSED){totalCount} } } }`

    ## ▶ 스타터 쿼리
    ```graphql
    query IssueCounts {
  viewer {
    repositories(first: 50, orderBy:{field:UPDATED_AT, direction:DESC}) {
      nodes {
        name
        open: issues(states: OPEN) { totalCount }
        closed: issues(states: CLOSED) { totalCount }
      }
    }
  }
}
    ```
