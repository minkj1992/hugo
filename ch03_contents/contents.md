# contents

## 콘텐츠 소스 구성
hugo에서 콘텐츠는 렌더링 된 웹사이트를 반영하는 방식으로 구성되야 합니다.

기본적으로 모든 수준에서 `중첩된 콘텐츠`를 지원하지만 **최상위 수준 `content/<DIRECTORIES>`는 특별하게 취급됩니다.**(콘텐츠 유형)


## page bundles
> [Page 리소스](https://gohugo.io/content-management/page-resources/)에 대한 그룹핑

```bash
.
└── content
    └── about
    |   └── index.md  // <- https://example.com/about/
    ├── posts
    |   ├── firstpost.md   // <- https://example.com/posts/firstpost/
    |   ├── happy
    |   |   └── ness.md  // <- https://example.com/posts/happy/ness/
    |   └── secondpost.md  // <- https://example.com/posts/secondpost/
    └── quote
        ├── first.md       // <- https://example.com/quote/first/
        └── second.md      // <- https://example.com/quote/second/
```
