    # Problem 26. 내 사용자 정보(me)

    **Endpoint**: GitHub

    ## 🎯 목표
    `viewer { login, name, bio }`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query Me {
  viewer {
    login
    name
    bio
  }
}
    ```
## 💡 힌트/주의
Authorization 헤더에 `Bearer <TOKEN>` 필요. Endpoint: https://api.github.com/graphql
