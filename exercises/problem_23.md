    # Problem 23. Alias: 동일 타입 두 번 조회

    **Endpoint**: SWAPI

    ## 🎯 목표
    `person(personID:1)`과 `person(personID:4)`를 `luke`, `vader` 별칭으로 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query TwoPersons {
  luke: person(personID: 1) { name }
  vader: person(personID: 4) { name }
}
    ```
