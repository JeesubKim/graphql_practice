    # Problem 20. SpaceX pagination 흉내 (offset)

    **Endpoint**: SpaceX

    ## 🎯 목표
    `launchesPast(limit:$limit, offset:$offset)`로 페이지 이동을 구현하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query LaunchesPage($limit: Int!, $offset: Int!) {
  launchesPast(limit: $limit, offset: $offset) {
    mission_name
    launch_year
  }
}
    ```
## 🔧 Variables (예시)
```json
{"limit":5,"offset":0}
```
