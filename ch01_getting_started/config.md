# Hugo Config
> hugo 사이트를 구성하는 방법

## 단일 파일

구성 파일 새롭게 지정 방법

```bash
hugo --config a.toml,b.toml,c.toml
```

## /config (디렉토리)

```
├── config
│   ├── _default
│   │   ├── config.toml
│   │   ├── languages.toml
│   │   ├── menus.en.toml
│   │   ├── menus.zh.toml
│   │   └── params.toml
│   ├── production
│   │   ├── config.toml
│   │   └── params.toml
│   └── staging
│       ├── config.toml
│       └── params.toml
```

`hugo --environment staging`을 통하여 단계를 나눌 수 있다.(prod, stag..)
