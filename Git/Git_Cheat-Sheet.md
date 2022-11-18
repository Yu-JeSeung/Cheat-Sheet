# How to use Git
## 01. 기본적인 셋팅
```bash
git config --global core.autocrlf true
git config --global core.safecrlf false
git config --global core.editor "code --wait"
git config --global user.name yu
git config --global user.email wptmd97@naver.com
cat ~/.gitconfig            # 깃 설정 확인
```

---

## 02. 프로젝트의 시작
```bash
* 새로운 폴더 생성
git init [directory name]

* 존재하는 레퍼지토리 복사
git clone [url]
```

---

## 03. 커밋하기
```bash
* Add *
git add .       # 현재 위치의 모든 파일 추가
git add [해당 파일 or 폴더 이름]

** Commit **
git commit -m 'commit message'

*** Add + Commit ***
git commit -am 'commit message'
```

---

## 04. 브랜치
```bash
git branch                      # 브랜치 확인
git branch [new-branch-name]    # 새로운 브랜치 생성
git checkout [branch]           # 브랜치 생성
git checkout -b [new-branch]    # 새로운 브랜치 생성 + 이동
git branch -d [branch]          # merge 한 브랜치 삭제
git branch -D [branch]          # merge 안한 브랜치 삭제
```

---

## 05. 병합
<img width="200" alt="image" src="https://user-images.githubusercontent.com/88806404/202662718-6cc0fe30-3696-446a-aa73-8b768a3b862c.png">

```bash
git checkout [main branch]
git merge [병합할 branch]
```