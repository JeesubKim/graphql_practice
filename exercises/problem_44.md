    # Problem 44. Fragment로 사용자 프로필 재사용

    **Endpoint**: GitHub

    ## 🎯 목표
    `fragment UserProfile on User { login name bio }`를 정의하고 여러 쿼리에서 사용.

    ## ▶ 스타터 쿼리
    ```graphql
    fragment UserProfile on User {
  login
  name
  bio
}
query MyFollowers {
  viewer { followers(first: 5) { nodes { ...UserProfile } } }
}
    ```
