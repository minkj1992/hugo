# Using a Git Submodule for theme(hugo, Jeky)

휴고, 지킬2에 대한 저장소가 있고 다른 저장소를 사용하려면 테마 저장소를 git submodule로 설정해야합니다.

hugo는 자체 모듈 관리 시스템을 가지고 있어, 빠르고 더 많은 가능성을 제공합니다. [hugo 모듈 사용 튜토리얼](https://dev.to/craftsmandigital/hugo-modules-for-dummies-42j9)

- `git submodule <Repo to be added as submodule> <path to theme>`

**만약 theme의 내용을 변경하고 싶고, 이를 내가 생성한 repo에 push하고 싶다면, update를 사용하면 된다.**

- `git submodule update --remote`

This is also how you update a third-party theme that you have installed as a submodule.

**하지만 종속성 관리를위한 git submodule은 불편한 방법 -> hugo module 사용**


