    # Problem 1. 모든 국가 코드/이름/대륙 코드

    **Endpoint**: Countries

    ## 🎯 목표
    모든 국가의 `code, name, continent.code`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query AllCountries {
  countries {
    code
    name
    continent { code }
  }
}
    ```
