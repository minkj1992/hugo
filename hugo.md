# what is hugo?

## `Hugo` 기능

- 개발 시, `LiveReload`를 통한 runtime 렌더링
- 정적 웹 사이트 렌더링이기 때문에, 모든 곳에서 Hugo 호스팅 가능

# Hugo basic
> https://gohugo.io/getting-started/

`hugo server`를 사용하면, LiveReload기능을 활용가능합니다. 

> Hugo는 템플릿을 `<script>`닫기 전에 LiveReload 를 삽입하므로 이 `</body>`태그가 없으면 작동하지 않습니다.

`hugo`를 사용하면 /public으로 정적 사이트 빌드가 가능합니다. 다만 해당 명령어는 기존에 생성되었던 /public을 삭제하지 않기 때문에 미리 /public을 삭제해 주어야 합니다. (또는 flag 활용)