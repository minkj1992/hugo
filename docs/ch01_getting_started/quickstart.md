## hugo 튜토리얼
```bash
hugo version
hugo new site quickstart
```

```bash
cd quickstart
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
echo 'theme = "ananke"' >> config.toml 
```

- 글 작성
  - `hugo new content/<CATEGORY>/<FILE>.<FORMAT>`

```bash
hugo new posts/my-first-post.md
```

- ./content/posts/my-first-posd.md 생성

```md
---
title: "My First Post"
date: 2020-10-30T22:47:29+09:00
draft: true
---
```

```bash
hugo server -D
```

- 사이트 구성
  - config.toml 편집

- 정적 페이지 작성

```bash
hugo -D

# ./public 생셩
```