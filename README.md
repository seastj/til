# Git

- Git 은 파일의 버전을 관리하는 툴

## Git 설치

- https://git-scm.com

![Image](https://github.com/user-attachments/assets/eaedf47b-7126-455a-9516-dd73403f0d07)
![Image](https://github.com/user-attachments/assets/3e3928bc-1655-41ec-ba9d-5663966db54b)
![Image](https://github.com/user-attachments/assets/c6b1444d-7284-41fd-b3a7-985e55279d42)

- `아래는 반드시 VSCode 설치하고 나서 진행하여야 함. (목록 확인 필요)`
  ![Image](https://github.com/user-attachments/assets/fe7ef510-011f-46b5-8b5d-bae7fcb86afc)
- 나머지는 기본값으로 설치완료함.

## Git 사용자 설정

- VSCode 에서 기본 터미널을 `Git Bash` 로 설정함.
- 터미널 실행 단축키 : `Ctrl + ~`
- 셋팅아이콘 선택 > Setting 메뉴 선택
  ![Image](https://github.com/user-attachments/assets/1ed4cfc1-3ee1-4f63-8176-bf7ca37600f5)

- 검색에 `Terminal default` 입력 > `Git Bash` 목록 선택
  ![Image](https://github.com/user-attachments/assets/7e7d8fd1-b01e-4f60-960a-0e5c100c28ec)

## Git 정보 확인 및 셋팅 (터미널에서 진행함)

- Git 버전 확인

```Bash
git --version
```

- 기본 브랜치명을 `main` 으로 설정하기(초기 설치시 master 로 되어있음.)

```bash
git config --global init.defaultBranch main
```

- Enter 키를 통일시킴(맥, 윈도우, 리눅스가 Enter키, 줄변경이 달리 처리됨)

```bash
git config --global core.autocrlf true
```

-깃 수정내역, 즉 commit 시 메세지 상세 남기기(VSCode 로 작성하도록 셋팅)

```bash
git config --global core.editor "code --wait"
```

- 사용자 설정 (아이디, 이메일)

```bash
git config --global user.name "아이디"
git config --global user.email "아이디@gmail.com"
```

```bash
git config --global user.name
git config --global user.email
```

# GitHub

- 회원가입(https://github.com) : 구글계정
- 예제 til_git 저장소 생성 (생략)

## GitHub 사용자 계정 보안 설정

- 초기 설정시 다음 내용을 필수로 확인한다

  - `자격 증명 관리자` > Window 자격 증명 탭 > Git 관련 제거
    ![Image](https://github.com/user-attachments/assets/b02c65ac-d7b1-462b-b306-aee19ac17c31)

- 깃허브 자격증명 등록은 git push 진행되면 자동으로 로그인 팝업이 출력됨.

## Git 작업 및 GitHub 연결 작업 진행

### 1. 최초 프로젝트 관리를 Git 으로 설정

```bash
git init
```

### 2. 현재 프로젝트 상태보기

```bash
git status
```

### 3. git으로 파일 추적하기

```bash
git add README.md
```
