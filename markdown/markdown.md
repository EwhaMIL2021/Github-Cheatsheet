# 마크다운 문법 

마크다운으로 필기하면 짱 편하고 깔끔하고 예쁩니다. 모두 마크다운 하세요!!!<br>
대체로 모든 마크다운 문서에서 적용되는 문법이지만, GitHub에서만 쓰이는 전용 마크다운 문법을 포함하고 있습니다.

### 목차

1. [제목](#💡제목)
2. [인용구](#💡인용구)
3. 

## 💡제목

```
# Head1
## Head2
### Head3
#### Head4
##### Head5
###### Head6
```

# Head1
## Head2
### Head3
#### Head4
##### Head5
###### Head6

이 이상은 안 됨!

## 💡인용구

```
> Quote
>> Sub quote1
>>> Sub quote2
>>>> Sub quote3
```

> Quote
>> Sub quote1
>>> Sub quote2
>>>> Sub quote3

인용구는 제목과 달리 `>`를 한도 끝도 없이(?) 추가할 수 있는 것 같습니다.

## 💡기본 서식

```
이건 그냥 글인데
이런 식으로 여러 줄에 걸쳐서 쓰면
띄어쓰기만 될 뿐 연달아서 써짐.
줄바꿈을 하고 싶으면 `<br>` 태그를 쓰거나<br>
엔터키를 두번

치면 다음줄로 넘어감!
```

이건 그냥 글인데
이런 식으로 여러 줄에 걸쳐서 쓰면
띄어쓰기만 될 뿐 연달아서 써짐.
줄바꿈을 하고 싶으면 `<br>` 태그를 쓰거나<br>
엔터키를 두번

치면 다음줄로 넘어감!

```
*이탤릭체* _이탤릭체_
**볼드체** __볼드체__
***둘 다***
<s>취소선</s>
`하이라이트` 작은따옴표 말고 `esc` 키 밑에 있는 애. 맥은 option(`⌥`)+`₩` 키
```

*이탤릭체* _이탤릭체_<br>
**볼드체** __볼드체__<br>
***둘 다***<br>
<s>취소선</s><br>
`하이라이트` 작은따옴표 말고 `esc` 키 밑에 있는 애. 맥은 option(`⌥`)+`₩` 키<br>

## 💡리스트

### 순서가 없는 리스트

```
- 첫번째
  - 첫번째 서브
    - 첫번째 서브의 서브
- 두번째
+ 플러스 기호도 되고
  + 1
  - 2
  - 3
* 별표도 됨
```

- 첫번째
  - 첫번째 서브
    - 첫번째 서브의 서브
- 두번째
+ 플러스 기호도 되고
  + 1
  - 2
  - 3
* 별표도 됨

### 순서가 있는 리스트

```
1. 첫번째
2. 두번째
3. 세번째
3. 네번째
```

1. 첫번째
2. 두번째
3. 세번째
3. 네번째

숫자 오타가 나도 자동으로 순서대로 지정됩니다.

### To-Do 리스트

```
- [ ] 할 일
- [x] 끝낸 일
```

- [ ] 할 일
- [x] 끝낸 일

## 💡코드

~~~~
```
일반 텍스트는 이런 식으로 쓰거나
```
~~~~

```
~~~~
이런 식으로 쓸 수도 있습니다.
~~~~
```

~~~~
소스코드를 쓰고 싶은 땐 ``` 옆에 언어 이름을 소문자로 적어주면, 예쁘게 하이라이팅 됩니다.

```python
print("Hello World")
```

```java
System.out.println("Hello World")
```

```c
printf("Hello World\n")
```
~~~~

```python
print("Hello World")
```

```java
System.out.println("Hello World")
```

```c
printf("Hello World\n")
```

~~~~
마찬가지로 터미널 명령어를 쓰고 싶으면 ``` 옆에 console이라고 씁니다.

```console
usr@ubuntu:~$ sudo update
```
~~~~

```console
usr@ubuntu:~$ sudo update
```

## 💡주석

```
<!--얘는 주석이라서 아래선 안 보일 것-->
```

<!--얘는 주석이라서 아래선 안 보일 것-->

## 💡구분선

```
---
***
___
```

---
***
___

## 💡링크

```
웹 링크는 이렇게: [여기로 들어가세요](https://github.com/EwhaMIL2021/Github-Cheatsheet/blob/main/markdown/markdown.md)
```

웹 링크는 이렇게: [여기로 들어가세요](https://github.com/EwhaMIL2021/Github-Cheatsheet/blob/main/markdown/markdown.md)

깃헙에서는 페이지 안에서도 링크를 달 수 있습니다.

```
[눌러보세요](#순서가-있는-리스트)
```

[눌러보세요](#순서가-있는-리스트)

## 💡GitHub 마크다운 문서에 이미지 추가

아무 레포지토리로 가서 `Issues` > `New issue`를 클릭합니다.

<img width="878" alt="스크린샷 2021-11-04 오후 6 36 30" src="https://user-images.githubusercontent.com/40985307/140291552-e45bf61b-122b-4a42-a306-52fbec5eab8f.png">

첨부할 이미지를 코멘트란으로 끌어오거나 복사해옵니다.

<img width="988" alt="스크린샷 2021-11-04 오후 6 39 18" src="https://user-images.githubusercontent.com/40985307/140292431-fbd55c6b-5d99-42cb-889c-5bd8227e5277.png">

그럼 이런 식으로 이미지 태그가 생기는데요, 이 태그를 복사합니다.
그리고 이미지를 첨부하고 싶은 마크다운 문서에 복사한 태그를 붙여넣기 합니다.

```
<img width="569" alt="스크린샷 2021-11-04 오후 6 43 35" src="https://user-images.githubusercontent.com/40985307/140292059-cd115891-6f61-4e9e-8369-6d0efd7f7fdc.png">
```

<img width="569" alt="스크린샷 2021-11-04 오후 6 43 35" src="https://user-images.githubusercontent.com/40985307/140292059-cd115891-6f61-4e9e-8369-6d0efd7f7fdc.png">

이 방법 외에도, 마크다운 문서와 같은 위치에 이미지를 저장해서 그 이미지의 링크를 다는 방법도 있습니다.

## 💡표

```
|Column1|Column2|
|---|---|
|항목1|항목2|

||Column1|Column2|Column3|
|---|:---|:---:|---:|
|**Row1**|왼쪽 정렬|가운데 정렬|오른쪽 정렬|
|**Row2**|빈칸도 됨||←이렇게|
```

|Column1|Column2|
|---|---|
|항목1|항목2|

||Column1|Column2|Column3|
|---|:---|:---:|---:|
|**Row1**|왼쪽 정렬|가운데 정렬|오른쪽 정렬|
|**Row2**|빈칸도 됨||←이렇게|

## 💡기타

### 이메일 연결

```
[Contact Me📩](mailto:user@email.com)
```

[Contact Me📩](mailto:user@email.com)

