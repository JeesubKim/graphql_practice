    # Problem 2. 국가 코드로 상세 조회

    **Endpoint**: Countries

    ## 🎯 목표
    `$code`로 국가를 조회하여 `name, capital, emoji, languages.name`을 반환하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query GetCountry($code: ID!) {
  country(code: $code) {
    name
    capital
    emoji
    languages { name }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"code":"BR"}
```
