    # Problem 11. 영화 목록 pagination (first)

    **Endpoint**: SWAPI

    ## 🎯 목표
    `allFilms(first:$n)`의 `edges { node { title } }`와 `pageInfo`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query FilmsPage($n: Int!) {
  allFilms(first: $n) {
    pageInfo { hasNextPage endCursor }
    edges { cursor node { title } }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"n":3}
```
