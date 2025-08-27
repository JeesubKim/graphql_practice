    # Problem 25. Directive @include / @skip

    **Endpoint**: Countries

    ## 🎯 목표
    `@include(if:$withCurrency)`로 `currency` 필드를 조건부로 요청하세요.

    ## ▶ 스타터 쿼리
    ```graphql
    query CountriesMaybeCurrency($withCurrency: Boolean!) {
  countries {
    name
    currency @include(if: $withCurrency)
  }
}
    ```
## 🔧 Variables (예시)
```json
{"withCurrency": true}
```
