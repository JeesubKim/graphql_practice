    # Problem 8. 특정 영화의 제목과 개봉일

    **Endpoint**: SWAPI

    ## 🎯 목표
    `film(filmID:$id)`의 `title, releaseDate`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query FilmBasic($id: ID!) {
  film(filmID: $id) {
    title
    releaseDate
  }
}
    ```
## 🔧 Variables (예시)
```json
{"id":"1"}
```
## 💡 힌트/주의
SWAPI GraphQL Endpoint 사용: https://swapi-graphql.netlify.app/.netlify/functions/index
