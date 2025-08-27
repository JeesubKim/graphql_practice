    # Problem 49. Inline Fragment로 Issue/PR 통합

    **Endpoint**: GitHub

    ## 🎯 목표
    `search(type:ISSUE)`로 가져온 노드가 Issue/PR일 때 각기 다른 필드를 요청.

    ## ▶ 스타터 쿼리
    ```graphql
    query MixedIssues {
  search(type: ISSUE, query: "repo:facebook/react is:issue,pr", first: 10) {
    nodes {
      __typename
      ... on Issue { number title author { login } }
      ... on PullRequest { number title author { login } }
    }
  }
}
    ```
