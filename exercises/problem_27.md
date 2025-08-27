    # Problem 27. 내 레포 10개 이름/생성일

    **Endpoint**: GitHub

    ## 🎯 목표
    `viewer { repositories(first:10, orderBy:{field:CREATED_AT, direction:DESC}) { nodes { name createdAt } } }`

    ## ▶ 스타터 쿼리
    ```graphql
    query MyRepos {
  viewer {
    repositories(first: 10, orderBy: {field: CREATED_AT, direction: DESC}) {
      nodes { name createdAt }
    }
  }
}
    ```
