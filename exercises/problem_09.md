    # Problem 9. 행성 거주자 이름들

    **Endpoint**: SWAPI

    ## 🎯 목표
    `planet(planetID:$id)`에 사는 `residentConnection { residents { name } }`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query PlanetResidents($id: ID!) {
  planet(planetID: $id) {
    name
    residentConnection { residents { name } }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"id":"1"}
```
