    # Problem 48. Alias로 서로 다른 레포 2개 동시 조회

    **Endpoint**: GitHub

    ## 🎯 목표
    예: `react: repository(owner:"facebook",name:"react")`, `vue: repository(owner:"vuejs",name:"core")`

    ## ▶ 스타터 쿼리
    ```graphql
    query TwoRepos {
  react: repository(owner: "facebook", name: "react") { name stargazerCount }
  vue: repository(owner: "vuejs", name: "core") { name stargazerCount }
}
    ```
