    # Problem 21. Fragment: 국가 공통 필드 재사용

    **Endpoint**: Countries

    ## 🎯 목표
    `fragment CountryFields on Country { code name emoji }`를 정의하고 재사용하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    fragment CountryFields on Country {
  code
  name
  emoji
}
query CountriesFrag {
  countries { ...CountryFields }
}
    ```
