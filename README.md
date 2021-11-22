# Github-Cheatsheet
깃헙 팁 모음!

### TIPS 바로가기
1. [git 블로그 만들고 관리하는 법](https://github.com/EwhaMIL2021/Github-Cheatsheet/blob/main/git/blog.md)
2. [git terminal 명령어 모음](https://github.com/EwhaMIL2021/Github-Cheatsheet/blob/main/git/commands.md)
3. [Markdown 문법](https://github.com/EwhaMIL2021/Github-Cheatsheet/blob/main/markdown/markdown.md)

### 목차 바로가기

1. [GitHub 사이트에서 Repository 관리하기](#GitHub-사이트에서-Repository-관리하기)
2. [내 컴퓨터에서 Repository 관리하기](#내-컴퓨터에서-Repository-관리하기)
    - [로컬 저장소에서 원격 저장소로 파일 올리기](#로컬-저장소에서-원격-저장소로-파일-올리기)
3. [파일 합치기](#파일-합치기)


`Algorithm-Study` repository를 예시로 정리해보겠습니다.

## GitHub 사이트에서 Repository 관리하기

### STEP1. `fork`를 눌러 본인 계정으로 Repository를 가져옵니다.

<img width="968" alt="스크린샷 2021-11-03 오후 3 57 38" src="https://user-images.githubusercontent.com/40985307/140020072-de5a26e4-b69e-4317-a4c5-8ab084e4f4f8.png">


### STEP2. `Add file` > `Create new file` 또는 `Upload files`에 들어가서 파일을 추가합니다.

<img width="902" alt="스크린샷 2021-11-03 오후 4 03 33" src="https://user-images.githubusercontent.com/40985307/140020490-e78915e0-29ec-4189-8d8c-45b08a4e2682.png">

`Upload files`로 올리는 경우 본인 컴퓨터(`local repository`)에 있는 파일 또는 폴더를 올릴 수 있습니다.<br>
`Create new file`은 깃헙 사이트(`remote repository`) 안에서 파일을 생성하는 방법입니다.
예) `장혜정/test.py`: `장혜정` 폴더 아래 `test.py` 파일 생성

<img width="465" alt="스크린샷 2021-11-03 오후 4 05 41" src="https://user-images.githubusercontent.com/40985307/140020628-fe6e3e27-d643-46cf-a087-5906bb97aef3.png">

<img width="817" alt="스크린샷 2021-11-03 오후 4 10 26" src="https://user-images.githubusercontent.com/40985307/140024433-7750d9fd-2276-4a6e-9801-adfe1384da69.png">


### STEP3. 파일이 성공적으로 업로드가 되었다면 Pull request를 할 수 있습니다.

💡 Pull request는 내 repository의 변경사항을 여기 그룹 repository에 반영을 해달라고 요청하는 작업입니다!<br>

`EwhaMIL2021/Algorithm-Study`로 가서 `Pull requests`를 클릭합니다.

<img width="977" alt="스크린샷 2021-11-03 오후 5 03 15" src="https://user-images.githubusercontent.com/40985307/140026229-4e5690f9-1799-4709-b8af-bc0741fe9e21.png">

`New pull request`를 눌러줍니다.

<img width="1229" alt="스크린샷 2021-11-03 오후 5 10 48" src="https://user-images.githubusercontent.com/40985307/140027136-859507a9-f101-45c2-bec4-6599b09a2282.png">

그럼 위의 이미지처럼 이렇게 아무것도 안 나와있을 텐데요, `compare accross forks`를 클릭하고, 밑에 콤보박스가 뜨면 `head repository`를 본인 계정으로 되어 있는 repository를 선택합니다.

<img width="1222" alt="스크린샷 2021-11-03 오후 5 13 20" src="https://user-images.githubusercontent.com/40985307/140027669-44acb212-95e0-4fa2-b3f9-e25a0ae94fba.png">

<img width="1213" alt="스크린샷 2021-11-03 오후 5 14 41" src="https://user-images.githubusercontent.com/40985307/140027604-0fe16284-b636-4596-a22d-37dd70adbbde.png">

이제 `EwhaMIL2021/Algorithm-Study`와 `내계정/Algorithm-Study` 비교가 뜰텐데요, 잘 확인해보고 측 상단의 `Create pull request`를 누릅니다.

<img width="1222" alt="스크린샷 2021-11-03 오후 5 17 59" src="https://user-images.githubusercontent.com/40985307/140027812-45daeb15-b79f-41b8-a647-df1fa84be189.png">

자유롭게 커밋 메시지를 쓰고, `Create pull request`를 클릭하면 Pull request 작업이 성공적으로 끝납니다.👏👏👏

<img width="915" alt="스크린샷 2021-11-03 오후 5 21 02" src="https://user-images.githubusercontent.com/40985307/140028166-b5b57135-e407-4c46-bb6d-d6b22c0992da.png">



## 내 컴퓨터에서 Repository 관리하기

여기서부턴 git 명령어를 이용해 내 컴퓨터로 repository를 내려받아서 관리하는 방법입니다.<br>

git은 Linux 기반이기 때문에 Linux 또는 Mac 유저는 별도의 프로그램을 받지 않아도 되지만, Windows에서는 프로그램 패키지를 따로 다운로드 받는 게 편합니다(git 터미널이 좀 더 예쁨).
[여기서](https://gitforwindows.org/) 받으면 되고 설치 방법은 구글에 검색해보면 많이 나오므로 여기선 생략하겠습니다!!

git repository는 remote repository(원격 저장소)와 local repository(로컬 저장소)로 나뉩니다.<br>
**원격 저장소**는 깃허브 사이트를 통해 만든 저장소, **로컬 저장소**는 원격 저장소를 내 컴퓨터로 그대로 복사해온 걸로 이해하면 편합니다.
이때 이 복사해오는 작업을 **cloning**이라고 합니다.

### `clone`

깃헙 사이트에서 본인 계정의 `Algorithm-Study` repository 페이지로 가서, 원격 저장소의 링크 주소를 복사해주세요.

<img width="907" alt="스크린샷 2021-11-03 오후 5 40 56" src="https://user-images.githubusercontent.com/40985307/140030447-3a619c84-8c27-441c-92c5-266bd337bff0.png">

그런 다음 Git Bash 또는 터미널을 열어 저장소를 불러올 위치(예를 들어 `Desktop`)로 이동을 하고, 다음과 같이 입력합니다.

```console
$ cd Desktop/
```

```console
$ git clone {좀전에 복사한 링크 주소}
```

참고로 Windows나 Linux에선 `Shift`+`Insert` 키를 누르면 붙여넣기가 됩니다.


### 설정과 초기화(`config`)

이제 로컬 저장소 폴더로 이동합니다.

```console
$ cd Algorithm-Study/
```

<img width="395" alt="스크린샷 2021-11-03 오후 5 55 23" src="https://user-images.githubusercontent.com/40985307/140032206-33dd46c3-85ad-4d3c-a899-b727597e6517.png">

그럼 현재 위치 왼쪽에 `main` 또는 `master`라는 이름이 붙게 되는데, 이건 깃헙에서 자동으로 생성해준 기본 브랜치(`branch`) 이름입니다.
최근 들어선 보통 `main`으로 만들어지는데 간혹 `master`가 되는 경우도 있으므로 잘 체크를 해야 합니다.<br>

아래처럼 계정 정보를 알려줍니다.

```console
$ git config --global user.email "{내이메일(반드시 깃헙에 가입할 때 쓴거)}"
$ git config --global user.name "{내이름}"
```

윈도우 환경의 경우 로그인 창이 같이 뜨게 될 텐데, 그럼 일단 token이라는 글자가 보이는 버튼을 클릭합니다.

#### 토큰 생성

우측 상단에서 프로필 클릭 > `Settings` > `Developer settings` > `Personal access tokens` > `Generate new token` 순서로 클릭합니다.

![1](https://user-images.githubusercontent.com/40985307/140268378-ca6443d1-5338-4abc-bae4-53b15deaa712.png)
![2](https://user-images.githubusercontent.com/40985307/140268366-2662b3d7-999f-4c9d-a25c-b2bf1063021f.png)

만기일을 정하고(`No expiration`으로 설정하는 게 편합니다) `repo`에 체크를 해주면 repository 관련 모든 권한(읽기, 쓰기, 삭제 등등)이 부여된 토큰이 만들어집니다.

![3](https://user-images.githubusercontent.com/40985307/140268375-6e20b9b4-71e9-486b-915b-c0f00b0896f1.png)

앞으론 이 토큰이 비밀번호 대신이므로 토큰을 복사해둡시다.<br>
❗️이 토큰은 지금만 확인할 수 있기 때문에 반드시 복사를 해놓아야 합니다!!!<br>


다시 로그인 창으로 돌아와서, token 기입란에 방금 복사한 토큰 값을 붙여넣기 해줍니다.<br>
맥이나 리눅스에선 조금 방법이 다른데요,
먼저 맥은 첫 push 작업을 할 때 토큰 값을 입력하면 키체인이라는 시스템에 자동으로 저장이 됩니다.
이 부분은 아래에서 정리해보겠습니다.<br>
그리고 리눅스는 [이 글](https://blog.naver.com/wkdgpwjd007/222547558728)을 참고해주세요!


### 로컬 저장소에서 원격 저장소로 파일 올리기

이제 대망의(!) 파일 올리는 기본 명령어 모음입니다.
이 명령어들만 외우고 있어도 어디 가서 "나는 git을 쓸 줄 안다!"라고 말할 수 있습니다.ㅎㅎ<br>

git에서 파일을 업로드하는 프로세스는 간단히 `pull` → `add` → `commit` → `push` 순서로 이뤄집니다.

#### `pull`

```console
$ git pull {원격 저장소 주소(기본값: origin)} {브랜치 이름(기본값: main 또는 master)}
```

`pull` 명령어는 원격 저장소가 로컬 저장소보다 최신 상태일 때, 로컬 저장소로 원격 저장소 상태를 불러와서 두 저장소를 동기화 시켜주는 명령어입니다.
만약 두 저장소의 상태가 같으면 이 명령어를 써도 아무 일이 안 일어나겠죠?<br>
로컬 저장소에서 원격 저장소로 파일을 올리기 전에 `pull`을 하지 않으면 파일 간 충돌이 발생할 수 있어서, 되도록 `pull`을 가장 먼저 해주는 게 좋습니다. 개인 repository를 혼자서만 관리하는 경우엔 안 해도 되지만, 특히나 협업을 할 때는 꼭 필요한 작업입니다.

#### `status`와 `add`

```console
$ git status
$ git add {파일명1} {파일명2} ... {파일명n}
$ git add --all
```

`git status`는 로컬 저장소에서 원격 저장소로 업데이트 작업을 수행할 파일 변경 사항이 있는지 확인하는 명령어입니다.
새 파일이 추가되거나 기존 파일이 수정 또는 삭제된 경우에 빨간 글씨로 해당 파일 목록이 뜨게 됩니다.<br>
전체 파일에 아무런 변경 사항이 없는 경우엔 다음과 같이 뜹니다.
<img width="682" alt="스크린샷 2021-11-04 오후 4 11 56" src="https://user-images.githubusercontent.com/40985307/140272197-4d4098ac-ede6-44ac-a47f-d48c652ea033.png">

`add`는 이런 파일들을 업데이트 목록에 추가하는 명령어인데요,
파일 이름을 개별적으로 하나씩 입력해도 되고 `--all` 옵션을 줘서 바뀐 파일 모두를 한꺼번에 추가할 수도 있습니다.<br>
이렇게 파일을 추가한 다음에 다시 `git status`를 입력하면 아까 빨간 글씨로 뜨던 파일 목록이 이제는 초록 글씨로 뜨는 걸 확인할 수 있습니다.

#### `commit`

```console
$ git commit -m "{커밋 메시지}"
```

`commit`은 위에서 `add`한 뭔가 변경 사항이 있는 파일들의 변경 이력을 기록하는 명령어로, 체크포인트 같은 거라고 생각하면 됩니다.
커밋 기록을 통해 필요할 때 과거 파일 상태까지도 다시 확인할 수 있습니다.<br>
나중을 위해선 한 번 커밋 할 때마다 커밋 메시지를 잘 쓰는 연습도 조금 중요한데요, 커밋 메시지에는 주요 변경 사항을 간단하게 요약해서 쓰는 게 좋습니다.

#### `push`

```console
$ git push {원격 저장소 주소} {브랜치 이름}
```

`push`는 최종적으로 `commit`을 마친 변경 사항을 원격 저장소에다가 업데이트하는 명령어입니다.
`push` 작업이 성공적으로 끝나면 GitHub 사이트의 원격 저장소에 로컬 저장소의 변경 사항이 똑같이 적용된 것을 볼 수 있습니다.

참고로 맥에서 `push` 명령어를 입력하고 나면 비밀번호를 치라고 뜰 텐데요, 여기에 아까 전에 복사해놨던 토큰을 붙여넣기 하면 됩니다.
보통 처음 한 번 입력하면 알아서 저장이 되는데 안 되는 경우엔 [이 글](https://blog.naver.com/adamdoha/222469955555)을 참고하면 좋을 것 같아요.

#### 요약

```console
$ git pull origin main
$ git status
$ git add test.py
$ git commit -m "add test.py"
$ git push origin main
```


## 파일 합치기

`Algorithm-Study`처럼 다수가 함께 쓰는 저장소에서는 여러 사람의 파일을 합쳐야 할 일이 생깁니다.
파일을 합치는 방법에는 여러 가지 방법이 있는데요,
로컬 저장소에서 `pull`을 한 다음에 `pull` 작업을 완료했다는 사실을 `commit` 및 `push`하는 방법이 있고
필요에 따라선 `merge` 명령어를 사용해서 합치는 방법도 있습니다.<br>

여기선 누군가의 `Pull request`가 있을 때 웹에서 간단히 합치는 법을 정리해볼게요.

마침 리퀘스트가 하나 있어서 캡처해봤습니다.
`Pull requests`에 들어가서 `Open`되어 있는 리퀘스트를 클릭합니다.
<img width="897" alt="스크린샷 2021-11-04 오후 4 36 40" src="https://user-images.githubusercontent.com/40985307/140275007-9a250cfa-257a-46b4-84c0-7bc7603fbcab.png">

그런 다음 `Merge pull request` > `Confirm merge` 순으로 클릭하고 메인 페이지로 돌아가면,

<img width="558" alt="스크린샷 2021-11-04 오후 4 37 44" src="https://user-images.githubusercontent.com/40985307/140274998-e5148b59-e412-4e61-b80e-031881c30cb5.png">
<img width="617" alt="스크린샷 2021-11-04 오후 4 37 15" src="https://user-images.githubusercontent.com/40985307/140275005-c7fc7eaf-bc61-45da-b8ed-6fcdfaaa7102.png">

이렇게 merge가 잘 반영돼 있는 것이 보입니다.
<img width="616" alt="스크린샷 2021-11-04 오후 4 49 37" src="https://user-images.githubusercontent.com/40985307/140276369-57193dc5-7df9-4961-8284-8ad76480d968.png">
