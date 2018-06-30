# 설치 및 최초 설정
- [설치](https://git-scm.com/book/ko/v2/%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-Git-%EC%84%A4%EC%B9%98)
- [최초 설정](https://git-scm.com/book/ko/v2/%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-Git-%EC%B5%9C%EC%B4%88-%EC%84%A4%EC%A0%95)
Git 설치는 사람들이 많이 쓰는 최신 운영체제를 쓰고 있다면 무척 간단하다. 이 [링크](https://git-scm.com/download) 에서 운영체제 별로 설치 파일을 다운로드해서 실행해 설치하면 된다. 만약 Mac이나 Linux를 쓰고 있다면 HomeBrew나 yum, apt등으로 설치도 가능하다. 만약 GitHub를 사용하다면 추천하는 프로그램은 [GitHub Desktop](https://desktop.github.com/)으로 GitHub에서 직접 만든 프로그램이다. GitHub와 연동이 완벽해서 원래 이 프로그램이 없었다면 GitHub에 푸시하기 위해서 별도의 설정을 해줘야 하는데 이 프로그램은 이중 인증이나 SSH key 같은 걸 신경 쓸 필요가 없도록 편하게 만들어져 있다. Git을 설치하고 이 프로그램을 연동해서 사용하면 좋을 것이다. 물론 Git 기능을 쓰기 위해 GitHub Desktop을 설치할 필요는 전혀 없다. 첫 링크에서 Git을 받아서 설치해도 Git의 모든 기능을 쓸 수 있다.

Git을 설치하고 사용하기 위해 반드시 Git에게 자신의 이름과 이메일을 알려줘야 한다. 터미널을 켜고 아래의 명령어를 입력하자.

```sh
$ git config --global user.name "Gildong Hong"
$ git config --global user.email "email@example.com"
```

`git config` 명령어는 git 설정을 관리하는 명령어다. `--global`은 전역 설정을 의미한다. 이름은 틀려도 되지만 이메일은 정확하게 입력해야 하는데 왜냐하면 커밋에 이름과 이메일이 기록된다. 따라서 이 커밋을 누가 했는지 추적하는데 이메일이 사용된다. GitHub에서도 커밋에 따른 사용자를 매핑하기 위해 이메일을 쓴다.