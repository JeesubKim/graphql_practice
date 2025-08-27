    # Problem 15. SpaceX 최근 발사체 5개

    **Endpoint**: SpaceX

    ## 🎯 목표
    `launchesPast(limit:5)`의 `mission_name, launch_date_utc`를 조회하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query LastLaunches {
  launchesPast(limit: 5) {
    mission_name
    launch_date_utc
  }
}
    ```
## 💡 힌트/주의
Endpoint: https://api.spacex.land/graphql/
