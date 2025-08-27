    # Problem 19. SpaceX payload 정보

    **Endpoint**: SpaceX

    ## 🎯 목표
    `launchesPast(limit:3)`에서 `payloads { nationality, type }`를 가져오세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query Payloads {
  launchesPast(limit: 3) {
    mission_name
    payloads { nationality type }
  }
}
    ```
