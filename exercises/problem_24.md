    # Problem 24. Inline Fragment: Node 인터페이스

    **Endpoint**: SWAPI

    ## 🎯 목표
    `node(id:$id)`로 가져온 대상이 Film일 때만 `title`을 요청하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query NodeMaybeFilm($id: ID!) {
  node(id: $id) {
    id
    ... on Film { title }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"id":"ZmlsbXM6MQ=="}
```
## 💡 힌트/주의
id는 글로벌 Relay ID입니다. GraphiQL에서 film의 `id`를 먼저 조회해 사용하세요.
