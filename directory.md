# hugo directory
> https://gohugo.io/getting-started/directory-structure/

- `hugo new site <>`

```bash
.
├── archetypes  # 콘텐츠 타입
├── config.toml # 또는 config/
├── content # 웹사이트에 게시될 모든 콘텐츠
├── data # 사용할 모든 데이터 (ex. 음반 리스트, csv 등등..)
├── layouts ## 렌더링 방식 지정 (list, home, detail)
├── static # css, javascript
└── themes
```

이외에도
- `config/`
  - 프로젝트 구성 지시문(레이아웃, 메뉴, 로그 등)
  - 간단한 로직에서는 config.toml사용
- `content/`
  - 웹사이트에서 사용할 모든 콘텐츠
  - 하위 디렉토리를 사용해 타입 지정 가능
- `assets`
  - Hugo Pipes에서 처리할 모든 파일 저장
  - 기본적으로 생성되지 않음