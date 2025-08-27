    # Problem 18. SpaceX 발사체 + 로켓 nested

    **Endpoint**: SpaceX

    ## 🎯 목표
    `launchesPast(limit:3)`의 `mission_name`과 내부 `rocket { rocket_name }`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query LaunchWithRocket {
  launchesPast(limit: 3) {
    mission_name
    rocket { rocket_name }
  }
}
    ```
