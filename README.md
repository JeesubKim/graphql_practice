# GraphQL 실전 연습 50문제 (실행 가능한 버전)

- 공개 GraphQL API를 대상으로 한 **실행 가능한** 50문제입니다.
- 난이도: 기초(1–10: Countries/SWAPI) → 중급(11–25: SWAPI/SpaceX) → 고급(26–40: GitHub) → 종합(41–50).
- 각 문제는 **엔드포인트**, **요구사항**, **스타터 쿼리/변수 템플릿**, **힌트/주의**를 포함합니다.
- `solutions/`에는 참고용 정답(예시 쿼리)이 포함되어 있으며, 실제 응답은 서비스 데이터에 따라 달라질 수 있습니다.

## 엔드포인트
- Countries: https://countries.trevorblades.com
- SWAPI GraphQL(Star Wars): https://swapi-graphql.netlify.app/.netlify/functions/index
- SpaceX (community): https://api.spacex.land/graphql/
- GitHub GraphQL: https://api.github.com/graphql  *(Personal Access Token 필요)*

## 사용 방법
1. 문제의 엔드포인트로 접속(또는 GraphiQL/Apollo Sandbox에서 URL 지정).
2. 문제의 스타터 쿼리/변수 템플릿을 복사해 실행.
3. 자신의 해답을 `solutions/solution_##.graphql` 또는 `.md`에 기록.

> GitHub API는 Authorization 헤더: `Bearer <YOUR_TOKEN>` 를 추가해야 합니다.
