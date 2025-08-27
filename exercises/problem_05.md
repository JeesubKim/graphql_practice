    # Problem 5. 영어 사용하는 국가

    **Endpoint**: Countries

    ## 🎯 목표
    언어 코드가 `en`인 나라의 `name`과 대륙 `name`을 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query EnglishSpeaking {
  countries(filter: { languages: { code: { eq: "en" } } }) {
    name
    continent { name }
  }
}
    ```
