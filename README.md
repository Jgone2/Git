## 개행 문자(NewLine) 설정

## macOS

```zsh
git config --global core.autocrlf input
```

## Windows

```bash
git config --global core.autocrlf true
```

# 사용자 정보

## 커밋(버전 생성)을 위한 정보 등록

```zsh
git config --global user.name 'Git Name과 동일하게 하는 것이 좋음'
```

```zsh
git config --global user.email 'Git 계정에 사용된 mail'
```

# 구성 확인

## 사용자 정보 확인

```zsh
git config --global --list
```

## git 버전 확인

```zsh
git --version
```

# 시작

## 현재 프로젝트에서 변경사항 추적(버전 관리) 시작

```zsh
git init
```

# 변경사항 추적 지정

## 변경사항을 추적할 특정 일을 지정

```zsh
git add index.html
```

## 모든 파일의 변경사항을 추적하도록 지정

```zsh
git add .
```

## Staged 상태 확인(git add 된 상태)

```zsh
git status
```

## Staged 상태 취소

```zsh
git rm --cached 파일명
```

# 버전 생성

## 메시지(-m)와 함께 버전을 생성

```zsh
git commit -m '프로젝트 생성'
git commit -m 'main.js 추가'
git commit -m 'index.html 수정'
```

## 버전 내역 확인

```zsh
git log
```

##commit 취소

```zsh
git reset HEAD~n
```

> git reset HEAD^ // 가장 최신 commit 취소  
>  git reset HEAD~3 // 최신 커밋 3개 취소
> git reset --hard

# GitHub 원격 저장소 연결

## origin이란 별칭으로 원격 저장소를 연결

```zsh
git remote add origin 원격저장소url
```

## origin이란 별칭의 원격 저장소로 버전 내역 전송

```zsh
git push origin master
```

# Branch

## branch 목록

```zsh
git branch
```

## 원격저장소에 있는 원격 branch 목록

```zsh
git branch -a
```

## branch 추가

```zsh
git branch branch명
```

## branch 삭제

```zsh
git branch -d branch명
```

## branch 이동

```zsh
git checkout 이동할branch명
```

## branch 생성 및 이동

```zsh
git checkout -b branch명
```

## branch 병합

```zsh
git merge branch명
```

> 💡 branch를 합병할 때, conflict(충돌)을 조심

## branch 병합 취소

```zsh
git merge --abort
```

## 원격 저장소로 버전 내역 전송

```zsh
git push origin 전송할branch명
```

# 복제(clone)

## 복제하기(repository 복제)

```zsh
git clone https://github.com/Jgone2/markdown.git
```

## 복제하기2

```zsh
git pull
```

> 💡 복제하기 전 원격 저장소연결이 필수적이며, 내가 로컬로 작업하고 있는 프로젝트와 병합을 위해 수행

## 작업하던 것 다른 곳에 임시 저장

```zsh
git stash   //git stash list로 목록확인도 가능
```

## 충돌
