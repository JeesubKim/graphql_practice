    # Problem 38. Release 버전 리스트

    **Endpoint**: GitHub

    ## 🎯 목표
    `releases(first:10)`의 `nodes { name tagName publishedAt }`

    ## ▶ 스타터 쿼리
    ```graphql
    query Releases($owner: String!, $name: String!) {
  repository(owner: $owner, name: $name) {
    releases(first: 10, orderBy:{field:CREATED_AT, direction:DESC}) {
      nodes { name tagName publishedAt }
    }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"owner":"vercel","name":"next.js"}
```
