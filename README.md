# k-cmd-wiki.github.io

https://k-cmd-wiki.github.io/

<br>
<br>
<br>

## 페이지 구조

.html 파일 하나만으로 구성된 SPA(싱글 페이지 애플리케이션) 웹사이트이며, 사용자의 컴퓨터에서 여기 깃허브 리포지토리의 데이터를 불러오는 식으로 동작합니다.

<br>

### 하위 페이지

링크의 맨 뒤에 해시(`#`) 기호와 함께 뭔 문자열이 있으면 이 리포지토리의 [pages 폴더](https://github.com/k-cmd-wiki/k-cmd-wiki.github.io/tree/main/pages) 안 해당 이름의 .md 파일이 불러와집니다.

예를 들어 https://k-cmd-wiki.github.io/#test >>> [pages/test.md](https://github.com/k-cmd-wiki/k-cmd-wiki.github.io/blob/main/pages/test.md) 와 같이 연결됩니다.

하위 페이지는 .md 파일을 불러와서 html 코드로 변환하는 식으로 동작합니다. 마크다운 문법(.md)을 사용하는게 미숙하신 분들은 [관련 나무위키 문서](https://namu.wiki/w/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4)를 읽고 오시면은 금방 익히실 수 있습니다. 

<br>

### chapters.txt

[홈화면](https://k-cmd-wiki.github.io/)의 버튼을 누르면 해시 주소값이 입력되어 하위 페이지로 연결되는걸 확인하실 수 있습니다.

[chapters.txt](https://github.com/k-cmd-wiki/k-cmd-wiki.github.io/blob/main/chapters.txt) 파일을 수정하여 이러한 버튼과 링크, 부제목을 추가/편집/제거할 수 있습니다.

chapters.txt 파일에서 세미콜론(`:`) 기호가 정확히 1개 배치되어 있는 텍스트는 버튼으로 인식됩니다. 세미콜론의 왼쪽이 버튼의 이름이며, 오른쪽은 연결할 하위 페이지의 파일명이자 해시 주소입니다. 예를 들어 아래 버튼은 https://k-cmd-wiki.github.io/#test 로 연결됩니다.
```
버튼 이름 : test
```

일반 텍스트는 부제목으로 인식됩니다.
```
이건 제목입니다. 예. 이게 제목이라고요.
```

일반적으로 부제목 밑에 버튼을 나열하는 식으로 페이지가 구성될겁니다. 이건 chapters.txt를 뜯어보시는게 이해가 더 빠를겁니다.
```
이건 제목입니다. 예. 이게 제목이라고요.
    버튼 이름 : test
    다른 버튼 이름 : a-s-d-f
    버튼 이름을 뭐로 하지 : QWERSDAFASDGREBHRSEG
```

(chapters.txt 파일은 줄단위로 파싱되며, 줄마다 맨 오른쪽과 맨 왼쪽에 있는 공백은 자동으로 제거됩니다. 비어있는 줄이나, 하이픈(`-`) 기호로만 이루어져 있는 줄이나, 공백으로만 이루어져 있는 줄 또한 자동으로 제거됩니다.)

<br>
<br>
<br>

## 편집 기여하기

### 멤버인 경우

관리자의 승인 없이 편집이 가능합니다.

파일을 추가하고 싶으면 Add file 버튼을 누르고, 파일을 수정하고 싶으면 펜 모양의 Edit this file 버튼을 누르면 편집창이 열립니다.

그리고 파일을 작성한뒤 저장하면, 위키 사이트에 즉시 반영됩니다. 끝.

<br>

### 멤버가 아닌 경우

> 더 상세히 적어주실 분 구함

1. 본인의 리포지토리로 포크
2. 포크한 걸 원하는대로 편집
3. 포크한 걸 풀리퀘스트
4. 관리자가 승인할때까지 대기

<br>
<br>
<br>

## 마크다운 문법 미리보기

https://k-cmd-wiki.github.io/preview
