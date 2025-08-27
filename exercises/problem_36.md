    # Problem 36. 내가 팔로우하는 사용자 10명

    **Endpoint**: GitHub

    ## 🎯 목표
    `viewer { following(first:10){ nodes{ login name } } }`

    ## ▶ 스타터 쿼리
    ```graphql
    query Following {
  viewer {
    following(first: 10) { nodes { login name } }
  }
}
    ```
