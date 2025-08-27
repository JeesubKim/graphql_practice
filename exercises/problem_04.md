    # Problem 4. 이름이 K로 시작하는 국가

    **Endpoint**: Countries

    ## 🎯 목표
    `countries(filter:{ name:{ regex:"^K"}})`에서 `code, name, continent.code`를 반환하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query StartsWithK {
  countries(filter: { name: { regex: "^K" } }) {
    code
    name
    continent { code }
  }
}
    ```
