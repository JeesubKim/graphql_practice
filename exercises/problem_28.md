    # Problem 28. 특정 레포의 Stars/Forks/Watchers

    **Endpoint**: GitHub

    ## 🎯 목표
    `repository(owner:$owner,name:$name)`의 `stargazerCount, forkCount, watchers.totalCount`

    ## ▶ 스타터 쿼리
    ```graphql
    query RepoStats($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    name
    stargazerCount
    forkCount
    watchers { totalCount }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"facebook","name":"react"}
```
