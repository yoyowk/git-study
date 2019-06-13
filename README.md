# 입문자를 위한 Git과 HTML&CSS
## 1일차
### 환경설정
- chrome 설치
- git 설치
- vs code 설치
### CLI 명령어 
- 디렉토리 생성 (mkdir)
- 디렉토리 이동 (cd)
- 빈 파일 생성 (touch)
- 내용 있는 파일 생성 (echo)
- 이름변경 및 이동 (mv)
- 복사 (cp)
- 디렉토리 삭제 (rmdir)
- 비어있지 않은 디렉토리 및 파일 삭제 (rm)
- 파일 및 디렉토리 목록 출력 (ls)
- 화면 지우기 (clear)
### git 명령어 학습
- 저장소 초기화 (git init)
- 사용자 이름 등록 (git config --global user.name "사용자 이름")
- 사용자 이메일 등록 (git config --global user.email "사용자 이메일 주소")
- 현재 상태 확인 (git status)
- index 영역으로 이동 /*커밋대기상태*/ (git add)
- 커밋 기록 생성 (git commit -m "커밋 메세지")
- 기본 에디터 수정 (git config --global core.editor "code --wait")
- 커밋 기록 수정 (git commit --amend)
- 커밋 로그 조회 (git log)
- 되돌리기 (git reset --hard 고유ID)
- 원격저장소 (git remote add origin 원격저장소 주소)
- 발행하기 (git push origin master)
- 일반 저장소에서 호스팅 저장소로 변경하기 
[youtube 영상](https://youtu.be/SNnfbf-LJz4)

## 2일차
### HTML 기본 구조
- DTD 선언(<DOCTYPE html>)
- html 요소 (html lang="ko-KR")
- head 요소 (문서 제목 및 메타데이터)
- 인코딩 선언 (meta charset="utf-8")
- body 요소 (본문 영역)

```html 
<!DOCTYPE html>
<html lang="ko-KR">
<head>
    <meta charset="UTF-8">
    <title>기본문서</title>
</head>
<body>
    환영합니다.
</body>
</html>
```

### HTML 요소
- 제목 요소 (h1 ~ h6)
- 문단 요소 (p)
- 강조, 분위기 전환 (b, i, strong, em)
- 줄바꿈, 수평선 (br, hr)
- 목록 요소 (ul, ol, li, dl, dt, dd)
- 하이퍼링크 (a, href 속성, target 속성, title 속성(툴팁))
- 이미지 (img, src 속성, alt 속성)
### CSS 개념 및 정의
- CSS는 Casecade Style Sheet의 약자로 스타일을 정의하기 위한 언어이다.
- 최신 표준은 CSS3라고 불리우는 새로 추가된 모듈이다.
- CSS의 중요한 개념은 겹침, 상속, 우선순위 이다.
- CSS를 이용하여 레이아웃 설계를 하기 위해서는 float, position, flex 등의 속성이 필요하다.
- CSS의 기본 문법은 선택자와 선언부로 구성되어 있다.
```css
    p{
        color:green;
        background-color:yellow;
    }
```
## 3일차
### CSS 선택자 및 박스모델
- 전체 선택자 (*)
- 요소 선택자 (tag 명령)
- class 선택자 (.class 명령)
- id 선택 (#id 명)
- width, height 속성 (박스의 가로 및 세로 크기)
- 테두리 (border)
- 여백 (padding, margin[auto 키워드를 사용할 수 있음])
- box-sizing 속성 (content-box, border-box)
- overflow 속성 (박스의 크기와 콘텐츠의 크기)
### 배치 관련 속성
- float 속성
> flaot 속성은 left와 right 값을 사용할 수 있으며 일반적인 흐름을 벗어나서 화면위에 떠있는 상태로 만들 수 있다. left나 right 값은 부모 영역을 기준으로 배치되며 각각 라인박스 안에서 배치된다는 특징이 있다. 또한 float 된 요소의 부모는 float 된 요소의 높이를 잃어버리기 때문에 부모요소에 overflow: hidden을 지정하여 문제를 해결할 수 있다.
- display: flex => [CSS Triks 참고자료](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
> 유연한 박스모델로 배치하고자 하는 요소의 부모 요소에 display 속성의 값으로 flex를 지정할 수 있다. 이때 flex가 지정된 요소의 자식 요소는 flex item의 역할을 담당하게 되고 flex-direction 속성에 지정된 방향으로 배치된다.
### 배경 관련 속성
- background-color (배경색)
- background-image (배경 이미지)
- background-repeat (배경 이미지 반복여부)
- background-position (배경 이미지 위치조절)
- backgruond-attachment (배경 이미지 고정여부)
- background-size (배경 이미지 크기)
- background 속성 (배경 관련 단축 속성)
## 4일차
### position 속성
- static(기본값)
- relative (상대배치)
- absolute (절대배치)
- fixed (고정배치 - 뷰포트 기준)
- sticky (relative + fixed 효과 - IE11 지원하지 않음)
### 애니메이션 관련 속성
- animation
 + animation-name (필수속성: 필수로 있어야 동작)
 + animation-duration (필수속성)
 + animation-fill-mode (시작 이후로 돌아갈 것인지, 멈출 것인지)
 + animation-delay
- transform
 + translate() (이동하는 기능)
 + scale()
 + rotate()
- transition
 + transition-property
 + transition-duration
 + transition-delay
