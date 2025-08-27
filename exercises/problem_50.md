    # Problem 50. 최종: 내 프로필 + 인기 레포 + 최근 PR/Issue

    **Endpoint**: GitHub

    ## 🎯 목표
    한 쿼리에서 viewer, 가장 Star 많은 레포 3개, 최근 PR 3개, 최근 Issue 3개를 가져오세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query Final {
  viewer {
    login
    name
    bio
    topRepos: repositories(first: 3, orderBy:{field:STARGAZERS, direction:DESC}) {
      nodes { name stargazerCount url }
    }
    recentPRs: pullRequests(first: 3, orderBy:{field:CREATED_AT, direction:DESC}) {
      nodes { title url createdAt }
    }
    recentIssues: issues(first: 3, orderBy:{field:CREATED_AT, direction:DESC}) {
      nodes { title url createdAt }
    }
  }
}
    ```
