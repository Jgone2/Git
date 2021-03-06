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
## branch 이동
```zsh
git checkout 이동할branch명
```
## 원격 저장소로 버전 내역 전송
```zsh
git push origin 전송할branch명
```

# 복제(clone)
## 복제하기(생성할 곳을 미리 지정)
```zsh
git clone https://github.com/Jgone2/markdown.git
```

## 충돌
