    # Problem 13. 우주선(Ships) 이름 리스트

    **Endpoint**: SWAPI

    ## 🎯 목표
    `allStarships(first:5)`에서 `name, model`을 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query Ships {
  allStarships(first: 5) {
    edges { node { name model } }
  }
}
    ```
