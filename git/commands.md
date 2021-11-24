# git terminal 명령어 

## 초기화

### 원격 repo (github에 있는 파일) 가져오기

```console
$ git clone https://github.com/USER/REPOSITORY.git
```

### 설정과 초기화

```console
$ git config --global user.email "github 가입할 때 쓴 이메일 주소"
$ git config --global user.name "내 이름"
```

## forked repository syncing

### stream 확인

```console
$ git remote -v
```

### upstream 추가

```console
$ git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
```

### ORIGINAL_REPOSITORY의 상태 가져오기 & 내 repo와 합치기

```console
$ git fetch upstream 
$ git checkout BRANCH
$ git merge upstream/UPSTREAM_BRANCH
```

## branch 명령어

### 현재 작업 중인 branch 확인

```console
$ git branch
```

### branch 이동 및 생성

```console
$ git checkout BRANCH_NAME  # 기본 브랜치명은 main 또는 master
$ git checkout -b NEW_BRANCH_NAME  # NEW_BRANCH_NAME라는 새 브런치 생성 후 자동 이동
```

### 특정 branch의 원격 repo 상태 가져오기

```console
$ git clone -b BRANCH_NAME --single-branch https://github.com/USER/REPOSITORY.git
```

### branch끼리 합치기

```console
$ git checkout BRANCH1  # BRANCH1으로 이동
$ git merge BRANCH2  # BRANCH1에 BRANCH2 내용 합치기
```

### branch 삭제

```console
$ git branch -d BRANCH_NAME
```

## 기본 명령어

기본 프로세스: (pull ->) add -> commit -> push

### 로컬 repo 상태 확인

```console
$ git status  # 변경된 파일들의 목록이 빨간색 글씨로 나타나게 됨
```

### 원격 repo 상태 가져오기(pull)

```console
$ git pull origin BRANCH
```

### 파일 변경사항 추가(add)

```console
# 변경된 파일명으로 추가
$ git add FILE_NAME
$ git add FILE_NAME_1 FILE_NAME_2 ... FILE_NAME_N

# 전체 변경사항(새 파일, 수정된 파일, 삭제된 파일) 추가
$ git add --all 또는 git add -A

# 새 파일 또는 수정된 파일만 추가
$ git add . 또는 git add *

# 수정 또는 삭제된 파일만 추가
$ git add --update 또는 git add -u
```

add 작업 후 `$ git status`를 해보면 변경된 파일들의 목록이 초록색 글씨로 나타나게 됨.

### 커밋(commit)

```console
$ git commit -m "COMMIT_MESSAGE"
```

commit 후에 `$ git status`를 해보면 더 이상 변경된 파일들의 목록이 뜨지 않음.

### 원격 repo에 올리기(push)

```console
$ git push origin BRANCH
```
