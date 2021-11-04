# Github-Cheatsheet
깃헙 팁 모음!

### 목차 바로가기

1. [GitHub 사이트에서 Repository 관리하기](#GitHub-사이트에서-Repository-관리하기)
2. [내 컴퓨터에서 Repository 관리하기](#내-컴퓨터에서-Repository-관리하기)
3. [Merge](


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

git repository는 **remote repository(원격 저장소)**와 **local repository(로컬 저장소)**로 나뉩니다.<br>
**원격 저장소**는 깃허브 사이트를 통해 만든 저장소, **로컬 저장소**는 원격 저장소를 내 컴퓨터로 그대로 복사해온 걸로 이해하면 편합니다.
이때 이 복사해오는 작업을 **cloning**이라고 합니다.

### `cloning`

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


### 설정과 초기화

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

### 토큰 생성



![1](https://user-images.githubusercontent.com/40985307/140268378-ca6443d1-5338-4abc-bae4-53b15deaa712.png)
![2](https://user-images.githubusercontent.com/40985307/140268366-2662b3d7-999f-4c9d-a25c-b2bf1063021f.png)
![3](https://user-images.githubusercontent.com/40985307/140268375-6e20b9b4-71e9-486b-915b-c0f00b0896f1.png)
