    # Problem 14. People 이름 필터링 흉내

    **Endpoint**: SWAPI

    ## 🎯 목표
    `allPeople(first:10)`을 가져와 클라이언트에서 이름이 'L'로 시작하는 사람만 필터링하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query PeopleFirst10 {
  allPeople(first: 10) {
    edges { node { name } }
  }
}
    ```
