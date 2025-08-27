    # Problem 12. 다음 페이지 가져오기 (after)

    **Endpoint**: SWAPI

    ## 🎯 목표
    `after:$cursor`로 다음 페이지를 요청하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query FilmsNext($n: Int!, $after: String) {
  allFilms(first: $n, after: $after) {
    pageInfo { hasNextPage endCursor }
    edges { cursor node { title } }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"n":3,"after":null}
```
## 💡 힌트/주의
첫 호출에서 받은 `pageInfo.endCursor` 값을 다음 호출의 `after`에 넣어보세요.
