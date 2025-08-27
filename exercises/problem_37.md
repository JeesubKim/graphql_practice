    # Problem 37. 추천 사용자(내가 팔로우하지 않음)

    **Endpoint**: GitHub

    ## 🎯 목표
    `search(type:USER, query:"followers:>100")` 등으로 후보를 가져오세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query SuggestUsers {
  search(type: USER, query: "followers:>100", first: 5) {
    nodes { ... on User { login name followers { totalCount } } }
  }
}
    ```
