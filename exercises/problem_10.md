    # Problem 10. 다스 베이더가 등장한 영화들

    **Endpoint**: SWAPI

    ## 🎯 목표
    `person(personID:$id)`의 `filmConnection { films { title } }`을 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query VaderFilms($id: ID!) {
  person(personID: $id) {
    name
    filmConnection { films { title } }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"id":"4"}
```
