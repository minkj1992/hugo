# Hugo 모듈
> [공식 hugo module](https://gohugo.io/hugo-modules/use-modules/)

- Hugo 모듈은 Go모듈로 구동됩니다.

## `Go`모듈

go-moduels는 vgo, dep, glide 등으로 파생되던 버전 관리의 표준을 제시하였으며, gopath를 더는 사용하지 않을 수 있도록 해주는 도구입니다. **즉 패키지간 종속성 관리를 golang team이 표준화하여 관리합니다.**

## Git submodule의 단점
> 재귀의 저주

첫번째 문제점은 git clone 시, 매번 각 submodule들을 init && update 해주어야 합니다. 어렵지는 않지만, 이를 뺴먹게 되면 failt to clone이 일어나는 귀찮은 스텝이 추가된다는 뜻입니다.

두번째 문제점은 git submodule은 제거시 어렵다는 단점이 있습니다. 사용했던 서브 모듈의 흔적을 지우기는 어려우며, 이에 대해서 "try then fry" 접근 방식을 채택하여 전체 프로젝트를 폐기하고 다시 복제하는 접근 방식을 쓰는 경우도 있습니다.

## Hugo module

모듈은 기본 프로젝트 또는 hugo에 정의된 7가지 구성요소 유형 중 하나 이상을 제공하는 작은 모듈입니다.

모듈의 출처와 마운트 할 디렉토리만 지정한다면 외부의 자원도 로컬의 것 처럼 사용가능합니다.

## Hugo Module tutorial
> [link](https://dev.to/craftsmandigital/hugo-modules-for-dummies-42j9)

- ./hugo_mod_tutorial

## Hugo Module tutorial2
> [link](https://www.hugofordevelopers.com/articles/master-hugo-modules-managing-themes-as-modules/)

- ./hugo_mod_tutorial2

```bash
mkdir hugo_module_tutorial2
cd hugo_mod_tutorial2
hugo mod init hugoModule2
```


- 주요 mod 명령어

```
hugo mod get    -프로젝트 구성에 선언 된 종속성 해결
hugo mod vendor -종속성 정보를 입력 _vendor하고 앞으로 사용
hugo mod graph  -모듈 식 종속성 그래프를 인쇄합니다.
hugo mod tidy   -프로젝트 구성에 선언 된 종속성에 따라 go.mod를 정리합니다.
```
