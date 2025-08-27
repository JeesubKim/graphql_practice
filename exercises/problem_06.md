    # Problem 6. 대륙 리스트와 국가 수

    **Endpoint**: Countries

    ## 🎯 목표
    모든 대륙의 `code, name`과 포함된 `countries.code`를 가져와 클라이언트에서 개수(count)를 구하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query ContinentsWithCountries {
  continents {
    code
    name
    countries { code }
  }
}
    ```
