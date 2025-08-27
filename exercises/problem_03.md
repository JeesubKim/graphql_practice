    # Problem 3. 아프리카 대륙 국가 목록

    **Endpoint**: Countries

    ## 🎯 목표
    `continent(code:"AF")` 아래 국가들의 `name, currency`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query AfricaCountries {
  continent(code: "AF") {
    name
    countries { name currency }
  }
}
    ```
