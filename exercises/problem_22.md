    # Problem 22. Fragment: 영화 공통 필드

    **Endpoint**: SWAPI

    ## 🎯 목표
    `FilmFields` fragment로 `title, releaseDate, director`를 재사용하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    fragment FilmFields on Film {
  title
  releaseDate
  director
}
query FilmsWithFragment {
  allFilms { edges { node { ...FilmFields } } }
}
    ```
