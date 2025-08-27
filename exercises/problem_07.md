    # Problem 7. 특정 국가의 통화와 이웃 정보

    **Endpoint**: Countries

    ## 🎯 목표
    `country(code:$code)`의 `name, currency, continent { name }`를 가져오세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query CountryCurrency($code: ID!) {
  country(code: $code) {
    name
    currency
    continent { name }
  }
}
    ```
## 🔧 Variables (예시)
```json
{"code":"KR"}
```
