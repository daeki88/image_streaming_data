

```python
# 영상/스트리밍 데이터와 얼굴 인식

## 프로그램 소개

- 데이터 유형
- 데이터의 중요성
- 데이터 수집/가공/분석 체험: 문서 통계 분석, 사진 
- 고급활용(얼굴, 사물 인식) 체험

## 보조 진행자

- 김찬준(11시 - 12시)
- 김진모(13시 - 15시)
- 황선재(11시 - 15시)
- 정아연(11시 - 12시)

## 진로체험의 중요성 및 영향

- 이 수업을 통해 데이터의 수집, 가공, 분석하는 방법을 체험함으로 데이터에 대한 막연한 생각들을 구체화한다.
- 데이터의 활용 예제를 직접 수행함으로 어렵지 않게 접근할 수 있다는 자신감을 얻는다.
- 이 경험을 바탕으로 넓고 다양한 직업에 대한 가능성을 엿볼 수 있다.
```

# 데이터

## 데이터 유형 및 응용

- 문서 데이터(정형: 표, 엑셀 데이터, 데이터 베이스(DB), 비정형: 웹 문서, SNS, 로그 데이터)
    - 연관성 분석: 연관 검색어([구글](https://www.google.com/search?q=날씨), 네이버)
    - 추천 시스템: 온라인 쇼핑([아마존](https://amazon.com))
    - 교통 정보: 실시간 빠른 길
    - 의료: [인공 지능 왓슨](http://www.sciencetimes.co.kr/?news=%EC%99%93%EC%8A%A8-%EC%A0%95%EB%B0%80%EC%9D%98%EB%A3%8C-%EC%8B%9C%EB%8C%80-%EC%97%B4%EA%B9%8C)(자연어 처리, 기계 학습)
- 영상 데이터(정지 영상, 동영상)
    - 사진 분류: [구글 "AI 이미지인식, 인간 능력 넘어설 것"](http://biz.chosun.com/site/data/html_dir/2017/03/26/2017032600545.html)
    - 사물 인식: [Object Recognition by Scene Alignment](http://bryanrussell.org/projects/recognitionBySceneAlignment/index.html)
    - 회화: [AI가 그린 그림 900만원에 팔려···예술 넘보는 인공지능](http://news.joins.com/article/19853826)
- 음성 데이터
    - 활용: 음성인식, 음성 변조, 작곡
    - 음성 비서: 애플 시리, 아마존 알렉사, 구글 어시스턴트

# 파이썬

파이썬(Python)은 1991년 프로그래머인 귀도 반 로섬(Guido van Rossum)이 발표한 고급 프로그래밍 언어이다. 파이썬이라는 이름은 귀도가 좋아하는 코미디 프로인 '몬티 파이썬의 하늘을 나는 서커스'(Monty Python's Flying Circus)에서 따온 것이라고 한다.
<img src="images/monty_python1.jpg"/>

## 파이썬 특징

- **배우기 쉽다.** 초보자가 배우기에 다른 언어에 비해서 쉽고 문법도 간단하다.
- **오픈소스이고 무료이다.** 자유롭게 배포할 수 있고 원하는대로 수정할 수 있으며 사용할 수 있다.
- **높은 수준(high-level)의 언어이다.** 사람들이 읽고 쓰기 편리한 언어를 말한다. 메모리 관리와 같은 저수준의 프로그래밍을 할 필요가 없다. 저수준(low-level)이라고해서 안좋다는 뜻이 아니고 초보자들이 접근하기 어려운 수준이라고 생각하면 될 것 같다.
- **호환 가능.** 윈도우즈, 리눅스, 맥 등 여러 운영체제에서 같은 코드를 실행할 수 있다.
- **인터프리터 형식.** `C/C++` 같은 프로그래밍 언어는 소스코드를 컴파일한 후 실행하는 과정을 거치지만 파이썬은 소스코드를 컴파일하는 과정이 필요없고 한 줄, 한 줄씩 실행할 수 있다.
- **플랫폼 독립적(Platform Independence)이다.** 외형적으로 인터프리터 방식이지만 내부적으로는 중간 언어인 바이트 코드 파일(.pyc)을 생성하기 때문에, 운영체제에 상관없이 실행할 수 있다.
- **객체지향적이다.** 객체를 중심으로 데이터와 함수를 프로그래밍하기 편리하다.
- **방대한 라이브러리.** 정규 표현식, 문서 생성, 단위 테스트, 스레드, 데이터베이스, 웹브라우저, CGI, FTP, HTML, WAV 파일, GUI등 방대한 양의 표준 라이브러리들을 사용할 수 있다.

## 파이썬 설치

파이썬 홈페이지 [https://www.python.org/](https://www.python.org/)에서 파이썬 [최신 버전](https://www.python.org/downloads/)을 다운받아 설치하는 방법과 아나콘다 프로그램을 [다운(https://www.continuum.io/downloads)](https://www.continuum.io/downloads)받아 설치하는 방법이 있다.

여기서는 아나콘다를 이용해서 파이썬을 설치해본다. 아나콘다를 설치하면 파이썬 프로그램뿐만 아니라 자주 사용되는 패키지들(Jupyter, Spyder, Numpy, SciPy, Pandas, matplotlib 등)이 기본적으로 설치되기 때문에 처음 사용자에게 편리하다. 또한 파이썬 버전과 호환되는 패키지들을 선택해서 설치하기 때문에 번거로움을 덜 수 있다.

## 아나콘다

### <a name="시스템종류확인"></a>시스템 종류 확인

아나콘다를 설치하기 전, 먼저 자신의 컴퓨터가 64비트인지 32비트인지를 확인하고, 맞는 프로그램을 다운로드하고 설치해야한다. 확인하는 방법은 제어판 - 시스템을 클릭해서 시스템 종류를 보고 확인할 수 있다

<img src="images/control_system.png" style="width: 600px"/>

### 아나콘다 다운로드

아나콘다 다운로드 홈페이지 [https://www.anaconda.com/download/](https://www.anaconda.com/download/)에 접속한다. 윈도우즈 파이썬 3.x 버전을 선택한다. 이것을 쓸 때 3.6버전이 최신 버전이다. 위에서 확인 시스템 종류에 맞는 버전을 클릭하여 다운로드 한다.

<img src="images/anaconda_download.png" style="width: 600px"/>

### 설치

다운로드 받은 파일을 클릭하여 설치를 시작한다.

<img src="images/anaconda_setup1.png" style="width: 600px"/>

아나콘다 프로그램을 사용자 혼자만 사용하게 할 것인지 모든 사용자가 사용하게 할 것인지를 선택하는 항목이다. 추천 항목인 Just Me를 선택한다.

<img src="images/anaconda_setup2.png" style="width: 600px"/>

아나콘다 설치 폴더는 자유롭게 선택할 수 있지만 폴더 경로에 빈 칸이 들어가면 문제가 될 수 있으므로 피해야 한다. 예를 들어 `c:\Program Files\Anaconda`와 같이 `Program`과 `Files`사이에 빈 칸으로 연결된 경로를 피해야 한다.

<img src="images/anaconda_setup3.png" style="width: 600px"/>

아나콘다에서 제공되는 파이썬 프로그램을 윈도우즈 기본 파이썬 프로그램으로 등록할지를 확인하는 항목이다. 다음 그림과 같이 선택한다.

<img src="images/anaconda_setup4.png" style="width: 600px"/>


## 명령어창에서 파이썬 실행

아나콘다(파이썬) 프로그램이 설치되었으면 실행창에서 간단한 파이썬 명령어들을 실행해보자. 아나콘다 실행창을 열어보자. 

1. 시작 버튼을 누르고
1. 프로그램 중에서 아나콘다(Anaconda)를 찾아서 누른다. 
1. 부메뉴 중에서 Anaconda Prompt를 눌러서 아나콘다 실행창을 연다.

![](images/anaconda_open_cmd1.jpg)

아나콘다 실행창에서 `python`을 실행한다.

<!--![](images/anaconda_prompt.png)-->
<img src="images/anaconda_prompt.png" style="width: 600px"/>

<!-- 만일 위와 같이 파이썬 실행 표시가 나오지 않는다면 파이썬 설치 경로를 시스템 환경에 설정해 줘야 한다. [시스템 경로 설정](#시스템 경로 설정)을 참고한다.

### <a name="시스템 경로 설정"></a> 시스템 경로 설정

제어판 -> 시스템 -> 고급 시스템 설정 -> 고급 탭 -> 환경변수를 클릭한다. 시스템 변수 항목 중에서 Path 변수를 선택 후 편집을 누른다. 새로 만들기를 눌러서 아나콘다(또는 파이썬) 설치 폴더 및 아나콘다(또는 파이썬) 설치 폴더/Scripts들을 새로 만든 후 확인을 계속 눌러서 창들을 닫는다. 그리고 명령어창을 ***새롭게*** 열어서 위의 명령어를 다시 실행해본다. -->

간단한 명령어들을 실행해보자.

<!--![](images/anaconda_prompt_simple_op.png)-->

<img src="images/anaconda_prompt_simple_op.png" style="width: 600px;" />

파이썬 실행을 끝내려면 `exit()`를 입력하고 엔터를 치든지, `Ctrl + Z`를 누르고 엔터를 치면 파이썬 프로그램을 닫는다.

<!--![](images/python_cmd_exit.jpg)-->

<img src="images/python_cmd_exit.jpg" style="width: 600px;" />

## 스크립트 파일 실행

명령어들을 한 줄 한 줄 입력해서 실행하기에 불편한 점이 많다. 여러 명령어들을 일괄적으로 실행하기위해서는 파일에 필요한 명령어들을 저장한다. 그리고 그 파일을 한꺼번에 실행할 수 있다. 또한 잘못된 곳이 있으면 그 파일 내용을 수정하여 다시 실행할 수 있다. 이러한 파일을 스크립트 파일이라고 부른다. 앞으로 실습을 위해서 작업 폴더를 만들어 보자.

### 실습 폴더 만들기

아나콘다 실행창에서 다음과 같이 실행한다.

1. `cd \`를 해서 맨 위의 폴더로 간다. `cd`는 change directory는 폴더의 위치를 변경하는 명령어이다. `\`는 역슬래시(백슬래시)라고 하며 한글 키보드 엔터키 바로 위에 &#8361;과 같은 키이다.
1. `mkdir work`를 해서 `work` 폴더를 새로 만든다. 이미 `work` 폴더가 있으면 `하위 디렉터리 또는 파일 work이(가) 이미 있습니다.`라는 메시지가 표시될 것이다. 무시하고 다음 단계로 넘어간다. `mkdir`은 make directory로 새로운 폴더를 만드는 명령어이다.
1. `cd work`를 해서 `work` 폴더로 들어간다.

<img src="images/cmd_mkdir.jpg" style="width: 600px;"/>

### 스크립트 파일 만들기

간단한 실습을 위해서 다음과 같이 메모장(notepad.exe) 프로그램을 이용해서 파일을 만들어 저장한다.

아나콘다 실행창에 `notepad example.py`라고 입력하고 엔터를 친다. 그러면 메모장이 실행되면서 `example.py` 파일이 없으면 새롭게 만들거냐고 물어볼 것이다. 그러면 `예`를 누른다. 그렇지 않고 이미 `example.py` 파일이 존재하면 그 파일이 열린다.

<img src="images/notepad_open.jpg" style="width: 600px;"/>

<img src="images/create_example_py.png" style="width: 600px;"/>

열린 메모장에서 다음과 같이 입력한 후 저장(Ctrl + S를 누르거나 매뉴의 파일 - 저장을 누른다)한다.

<img src="images/example_py.png" style="width: 600px;"/>

아나콘다 실행창에서 `python example.py`를 입력하여 실행하면 다음과 같은 결과를 확인할 수 있다.

<img src="images/example_py_result.png" style="width: 600px;"/>

메모장 `example.py` 내용을 숫자를 바꾸어 저장한 후, 아나콘다 실행창에서 `python example.py` 다시 실행하면 결과가 다르게 나오는 것을 확인할 수 있을 것이다.

간단한 실습을 위해서 메모장을 사용한 것이지 앞으로 프로그래밍을 할 때는 사용하지 않을 것이다. 파이썬 프로그래밍을 편하게 할 수 있는 전용 편집기 PyCharm을 사용할 것이다.

## 통합 개발환경 파이참(PyCharm)

파이썬 프로그래밍을 효율적으로 할 수 있게 도와주는 프로그램인 PyCharm 통합개발환경 Community Edition에 대해서 알아본다. PyCharm Community Edition은 무료이고 오픈소스이다. 파이참은 파이썬 편집을 할 때 필요한 함수들을 자동으로 완성해주는 기능 및 도움말도 쉽게 살펴 볼 수 있다. 또한 실행 및 디버깅도 쉽게 할 수 있고 파일의 버전 제어(svn, git) 기능도 사용할 수 있다.

### 파이참 다운로드

파이참 다운로드 홈페이지 https://www.jetbrains.com/pycharm/download/에 접속해서 Community Edition을 다운 받는다.

<img src="images/pycharm_download.png" style="width: 600px;"/>

### 파이참 설치

다운로드 받은 파일을 클릭하여 설치를 시작한다.

<img src="images/pycharm_setup1.png" style="width: 600px;"/>

설치 폴더를 정하는 화면이다. 기본 설정 폴더로 한다.

<img src="images/pycharm_setup2.png" style="width: 600px;"/>

32비트 또는 64비트를 설치할 건지 선택하는 화면이다. 아나콘다 설치시 살펴봤던 [시스템 종류 확인](#시스템종류확인)에서 확인한 정보를 이용해서 선택한다.

<img src="images/pycharm_setup3.png" style="width: 600px;"/>

파이참을 실행하면, 기존의 파이참 설정 파일을 가져올 건지를 물어보는 항목이다. 처음 설치하는 것이므로 `Do not import settings`를 선택한다.

<img src="images/pycharm_setup4.png" style="width: 600px;"/>

라이선스 동의 화면이다. `Accept`를 누른다.

<img src="images/pycharm_setup5.png" style="width: 600px;"/>

파이참 테마를 설정하는 부분이다. 기본 설정을 따른다.

<img src="images/pycharm_setup6.png" style="width: 600px;"/>

<img src="images/pycharm_setup7.png" style="width: 600px;"/>

새로운 프로젝트를 생성한다.

<img src="images/pycharm_setup8.png" style="width: 600px;"/>

새로운 프로젝트 위치와 이름을 설정한다. `C:\work\sample1`이라고  설정하자.

<img src="images/pycharm_setup9.png" style="width: 600px;"/>

### 파이참 테마 변경

파이참 기본 테마를 변경하는 방법에 대해 알아본다. File - Settings를 눌러서 Settings 팝업창을 띄운다.

<img src="images/pycharm_theme.png" style="width: 600px;"/>

Settings 창에서

<img src="images/pycharm_theme_darcula.png" style="width: 600px;"/>

1. Appearance & Behavior를 누르고
1. Apperance를 선택한다.
1. Theme 항목에서 원하는 항목을 선택하면 된다. 기본 설정은 IntelliJ이다. 앞으로 여기서는 Darcula 테마를 사용할 것이다.

다음은 Darcula 테마를 적용한 화면이다.

<img src="images/pycharm_theme_darcula_set.png" style="width: 600px;"/>

### 새로운 프로젝트 만들기 및 실행

파이참을 사용하기 위해서는 먼저 프로젝트를 만들어야 한다. 메뉴에서 File - New Project을 눌러서 새로운 프로젝트를 만든다.

<img src="images/pycharm_newproject.jpg" style="width: 600px;"/>

새로운 프로젝트 위치와 이름을 다음과 그림과 같이 `C:\work\ProjectExample` 폴더로 정한다.

<img src="images/pycharm_createproject.png" style="width: 600px;"/>

1. 오른쪽 `...`을 눌러서 원하는 폴더를 선택한다.
1. `c:\work` 폴더를 선택 후 확인을 누른다.
1. `Location:` 항목에서 `c:\work\ProjectExample`이라고 입력을 한다.

프로젝트에 새로운 파일을 만들어 보자.

<img src="images/pycharm_new_file.png" style="width: 600px;"/>

1. 왼쪽편에 있는 프로젝트 이름을 마우스 오른쪽 클릭하고
1. New를 누른 후
1. Python File을 누르면 팝업창이 뜬다.

<img src="images/pycharm_new_file1.png" style="width: 600px;"/>

1. `Name` 항목에 `FirstEx`라고 쓰고 확인을 누른다.

간단한 프로그램을 작성하고 실행해 본다.

<img src="images/pycharm_run_file.png" style="width: 600px;"/>

1. 편집창에 `print('Hello world, 안녕')`이라고 적는다.
1. 편집창에서 마우스 오른쪽 클릭하여 `Run FirstEx`를 누른다.
1. 편집창 아래에 결과 `Hello world, 안녕`이 보일 것이다.

프로젝트에 새로운 파일을 추가하고 싶으면 위와 같은 방법을 반복하면된다.


## 파일 이름

주의: 스크립트 파일 이름을 저장할 때 기존 모듈 이름으로 저장하고 import 모듈 하면 프로그램이 제대로 동작하지 않을 수 있다. 예를 들면 사용자가 파일 이름을 `mymodule.py`라고 저장했다고 하자. 그런데 파이썬이 이미 그와 같은 모듈을 갖고 있어서 사용자가 파이썬이 내장하고 있는 `mymoule` 모듈을 불러오려고 다음과 같이 쓰면 사용자가 저장했던 `mymoudle.py`가 불어와지게 되어 제대로 작동하지 않을 수 있다.

```python
import mymodule

....
....
```

어떻게 파일 이름을 지을 지 고민될 때는 원하는 파일 이름 뒤에 `Ex` 또는 자신의 영문 대문자를 사용하는 것도 좋은 방법이다. 예를 들면 파일이름을 `mymodule`이라고 짓고 싶을 때는 `mymoduleEx` 또는 `mymoduleDyoon`이라고 하면 크게 문제가 없을 것이다.

#  문서 데이터

## HTTP

HTTP는 **H**yper**T**ext **T**ransfer **P**rotocol의 약자로 인터넷을 통해 데이터를 주고 받기 위한 서버/클라이언트 모델을 따르는 프로토콜이다. 응용 수준의 규약(프로토콜)으로 TCP/IP 위에서 작동한다. HTTP는 HTML, 이미지, 동영상, 오디오, 텍스트 문서 등의 데이터를 전송할 수 있다.

웹 브라우저(클라이언트)를 통해 웹 사이트(서버)에 접속하여 원하는 정보를 보는 절차는 다음 그림과 같다.

<img src="images/http_client_server.png" style="width: 400px"/>

클라이언트에서 요청(request) 메시지를 보내면 서버에는 요청 정보를 처리하여 응답(response) 메시지를 보낸다. 요청 메시지와 응답 메시지 형식은 다음과 같다.

### 요청(request)

다음은 브라우저가 서버에게 요청하는 메시지의 예제이다.

```python
GET / HTTP/1.1\r\n
Host: www.google.com\r\n
User-Agent: python-requests/2.18.4\r\n
Accept-Encoding: gzip, deflate\r\n
Accept: */*\r\n
Connection: keep-alive\r\n
\r\n
```

요청 메시지는 요청 줄과 헤더, 메시지 몸통으로 구성되어 있다. 요청 줄은 요청 메소드(get, post, put, delete, head, options, trace), 요청 uri, http 버전이 나온다.
```python
GET / HTTP/1.1\r\n
```

#### 요청 메소드

메소드는 서버에게 어떤 종류의 요청인지 알려준다.

| 메소드 | 설명|
| --- | --- |
| GET | 서버에 정보를 요청한다.|
| POST | 폼(데이터)을 서버에 넘겨주기 위해서 사용한다.|
| PUT | 서버의 데이터를 업데이트하기 위해 사용한다.|
| DELETE | 서버 데이터를 삭제하기 위해서 사용한다.|
| HEAD | HTTP 헤더 정보만 요청한다. 해당 자원이 존재하는지 혹은 서버에 문제가 없는지 확인하기 위해서 사용한다.|
| OPTIONS | 웹서버가 지원하는 메소드의 종류를 알아본다.|
| TRACE | 클라이언트의 요청을 그대로 돌려보낸다.|

#### 요청 URI

통합 자원 식별자(Uniform Resource Identifier, URI)는 정보가 서버에 위치해 있는 주소를 가리킨다. 위의 예에서 `/`가 URI이다.

#### 요청 헤더

요청 줄 다음으로 나오는 것은 요청 헤더이다. 헤더는 브라우저 종류, 웹 페이지 언어, 서버 주소 등의 메타 데이터가 나온다. 자세한 것은 [HTTP/1.1 세부 명세](https://tools.ietf.org/html/rfc2616)를 확인한다.

### 응답(response)

브라우저를 통해서 서버에 요청을 하면 서버가 응답을 하면서 메시지를 보낸다. 아래는 응답 메시지 예제이다.

```python
HTTP/1.1 200 OK
'Date': 'Mon, 20 Nov 2017 01:11:02 GMT',
'Expires': '-1',
'Cache-Control':'private, max-age=0',
'Content-Type': 'text/html; charset=EUC-KR',
'P3P': 'CP="This is not a P3P policy! See g.co/p3phelp for more info."',
'Content-Encoding': 'gzip', 'Server': 'gws',
'Content-Length': '5065',
'X-XSS-Protection': '1; mode=block',
'X-Frame-Options': 'SAMEORIGIN',
'Set-Cookie': '1P_JAR=2017-11-20-01; expires=Wed, 20-Dec-2017 01:11:02 GMT; path=/; domain=.google.co.kr, NID=117=qpfOPSGFis-r3WpI7ejpkONxTkZj0W0LjhFgCJSmY3S4rGi2RFBjxHEvB_JvaWFw9OqLdP7TPDp9RxTU0VeVaJ0F5pR7jgcdmIFmL9G_XpGCnuotMM7p3V7yhxU-p3Kf; expires=Tue, 22-May-2018 01:11:02 GMT; path=/; domain=.google.co.kr; HttpOnly'
```

웹 브라우저를 이용하면 ***개발자 도구 메뉴***를 통해서 `http` 요청/응답에 대한 정보를 확인할 수 있다. 크롬인 경우는 `F12`를 눌러 개발자 도구를 열어 `Network` 탭을 클릭해보면 요청, 응답 메시지를 확인할 수 있다.

## HTML(HyperText Markup Language)

웹브라우저에서 사용되는 언어이다.

```html
<html>
<head>
<title>안녕하세요. 제목입니다.</title>
</head>
<body>
<h1>제일 굵은 글씨입니다.</h1>
<p>문단을 나타냅니다.</p>
몸통입니다.
<ul>
순서가 없는 리스트를 나타냅니다.
<li>하나</li>
<li>둘</li>
<li>셋</li>
</ul>

<ol>
순서가 있는 리스트입니다.
<li>일</li>
<li>이</li>
<li>삼</li>
</ol>
<table>
<thead>
<tr>
<th>이름</th>
<th>나이</th>
<th>고등학교</th>
<th>도시</th>
</tr>
</thead>
<tbody>
<tr>
<td>홍길동</td>
<td>18</td>
<td>한솔고</td>
<td>세종</td>
</tr>
<tr>
<td>홍길동</td>
<td>18</td>
<td>한솔고</td>
<td>세종</td>
<tr>
</tbody>
</table>
</body>
</html>
```

## 데이터 수집 및 파싱(Parsing)

### 웹 페이지 읽기
 
`requests` 모듈을 이용하여 웹 페이지를 읽어 올 수 있다.
 
- 다음(daum) 홈페이지에 접속해서 HTML 문서를 가져와 화면에 출력하는 예이다.


```python
import requests

resp = requests.get( 'http://daum.net' )
 
if (resp.status_code == requests.codes.ok):
    html = resp.text
html.split('\n')[0:10]
```




    ['<!DOCTYPE html>',
     '<html lang="ko" class="">',
     '<head>',
     '<meta charset="utf-8"/>',
     '<title>Daum</title>',
     '<meta property="og:url" content="https://www.daum.net/">',
     '<meta property="og:type" content="website">',
     '<meta property="og:title" content="Daum">',
     '<meta property="og:image" content="//i1.daumcdn.net/svc/image/U03/common_icon/5587C4E4012FCD0001">',
     '<meta property="og:description" content="나의 관심 콘텐츠를 가장 즐겁게 볼 수 있는 Daum">']



## 파싱(Beautiful Soup)

BeautifulSoup 모듈을 이용해서 웹 페이지에서 필요한 정보들을 찾아낼 수 있다.

- 설치

```python
pip install beautifulsoup4 # 또는
conda install beautifulsoup4 # 아나콘다를 이용할 경우
```

- BeautifulSoup 웹페이지 파싱

웹 문서를 입력받아 bs객체를 만든다. bs 객체를 이용하여 필요한 정보들에 접근해서 원하는 것들을 수집할 수 있다. 원하는 성분으로 접근하는 방법은 여러 가지가 있으나 select() 함수를 이용하는 방법이 있다. select 함수의 인자는 css selector 조합 문자열을 사용한다. css selector에 대한 자세한 설명은 [W3 Schools CSS Selector Reference](https://www.w3schools.com/cssref/css_selectors.asp)를 참조한다. 다음은 몇 가지 예를 보여준다.

| Selector | 예제 | 설명 | CSS 버전 |
| ---- | ---- | ----- | ---- | ----- |
|`.class` | `.intro` | `class="intro"`인 모든 성분 선택 | 1 |
|`#id` | `#firstname` | `id="firstname"`인 모든 성분 선택 | 1 |
| `*` | `*` | 모든 성분 선택 | 2 |
|`element` | `p` | `<p>` 성분 모두 선택 | 1 |
|`element, element` | `div, p` | `<div>` 또는 `<p>`를 갖는 모든 성분 선택 | 1 |
|`element element` | `div p` | `<div>` 성분 안에 `<p>` 성분을 갖는 모든 성분 선택| 1 |
|`element>element` | `div > p` | 부모가 `<div>`인 모든 `<p>` 성분 선택 | 2 |
|`element+element` | `div + p` | 바로 위의 부모가 `<div>`인 모든 `<p>` 성분 선택 | 2 |
|`element1~element2` | `p ~ ul`| `<p>` 바로 다음에 있는 `<ul>` 성분들 선택 | 3 |
|`[attribute]` | `[target]` | 속성이 `target`인 모든 성분 선택 | 2 |
|`[attribute=value]` | `[target=_blank]` | 속성이 `target`이고 `target`의 값이 `_blank`인 모든 성분 선택 | 2 |
|`[attribute~=value]` | `[title~=flower]` | `title`속성을 갖고 속성값이 `flower`단어를 포함하는 모든 성분들 선택 | 2 |
|`[attribute` &#124;`=value`] | `[lang` &#124; `=en`] | 속성이 `lang`이고 속성의 값이 `en`으로 시작하는 모든 성분 선택 | 2 |


```python
import bs4
 
html = "<html><head><title>제목</title></head><body>...생략...</body></html>"
bs = bs4.BeautifulSoup(html, 'html.parser')
bs.select('body')
```




    [<body>...생략...</body>]



- 네이버 금융 사이트에서 헤드라인 뉴스 제목 발췌


```python
import requests
import bs4
 
resp = requests.get('http://finance.naver.com/')
resp.raise_for_status()
 
resp.encoding='euc-kr'
html = resp.text
 
bs = bs4.BeautifulSoup(html, 'html.parser')
print(bs.prettify()[0:100], "\n.\n.\n.\n", bs.prettify()[-100:])

tags = bs.select('div.news_area h2 a') # 헤드라인 뉴스 제목
title = tags[0].getText()
print("헤드라인 제목: ", title)
```

    <html lang="ko">
     <head>
      <title>
       네이버 금융
      </title>
      <meta content="text/html; charset=utf-8" h 
    .
    .
    .
     , 이미지 리플레시 
    jindo.$Fn(mainPageDomReadyFn).attach(document, "domready");
      </script>
     </body>
    </html>
    헤드라인 제목:  "환율 부담, 지속되진 않을 것"
    

## 분석

### pandas
`pandas` 모듈은 데이터를 다루기 편리한 함수들을 제공한다.

#### 생성

- 엑셀 데이터 읽기


```python
import pandas as pd

df_excel = pd.read_excel('http://qrc.depaul.edu/Excel_Files/Presidents.xls'); df_excel
```




<div>
<style>
    .dataframe thead tr:only-child th {
        text-align: right;
    }

    .dataframe thead th {
        text-align: left;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>President</th>
      <th>Years in office</th>
      <th>Year first inaugurated</th>
      <th>Age at inauguration</th>
      <th>State elected from</th>
      <th># of electoral votes</th>
      <th># of popular votes</th>
      <th>National total votes</th>
      <th>Total electoral votes</th>
      <th>Rating points</th>
      <th>Political Party</th>
      <th>Occupation</th>
      <th>College</th>
      <th>% electoral</th>
      <th>% popular</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>George Washington</td>
      <td>8</td>
      <td>1789</td>
      <td>57</td>
      <td>Virginia</td>
      <td>69</td>
      <td>NA()</td>
      <td>NA()</td>
      <td>69</td>
      <td>842.0</td>
      <td>None</td>
      <td>Planter</td>
      <td>None</td>
      <td>100.000000</td>
      <td>NA()</td>
    </tr>
    <tr>
      <th>1</th>
      <td>John Adams</td>
      <td>4</td>
      <td>1797</td>
      <td>61</td>
      <td>Massachusetts</td>
      <td>132</td>
      <td>NA()</td>
      <td>NA()</td>
      <td>139</td>
      <td>598.0</td>
      <td>Federalist</td>
      <td>Lawyer</td>
      <td>Harvard</td>
      <td>94.964029</td>
      <td>NA()</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Thomas Jefferson</td>
      <td>8</td>
      <td>1801</td>
      <td>57</td>
      <td>Virginia</td>
      <td>73</td>
      <td>NA()</td>
      <td>NA()</td>
      <td>137</td>
      <td>711.0</td>
      <td>Democratic-Republican</td>
      <td>Planter, Lawyer</td>
      <td>William and Mary</td>
      <td>53.284672</td>
      <td>NA()</td>
    </tr>
    <tr>
      <th>3</th>
      <td>James Madison</td>
      <td>8</td>
      <td>1809</td>
      <td>57</td>
      <td>Virginia</td>
      <td>122</td>
      <td>NA()</td>
      <td>NA()</td>
      <td>176</td>
      <td>567.0</td>
      <td>Democratic-Republican</td>
      <td>Lawyer</td>
      <td>Princeton</td>
      <td>69.318182</td>
      <td>NA()</td>
    </tr>
    <tr>
      <th>4</th>
      <td>James Monroe</td>
      <td>8</td>
      <td>1817</td>
      <td>58</td>
      <td>Virginia</td>
      <td>183</td>
      <td>NA()</td>
      <td>NA()</td>
      <td>221</td>
      <td>602.0</td>
      <td>Democratic-Republican</td>
      <td>Lawyer</td>
      <td>William and Mary</td>
      <td>82.805430</td>
      <td>NA()</td>
    </tr>
    <tr>
      <th>5</th>
      <td>John Quincy Adams</td>
      <td>4</td>
      <td>1825</td>
      <td>57</td>
      <td>Massachusetts</td>
      <td>84</td>
      <td>NA()</td>
      <td>NA()</td>
      <td>261</td>
      <td>564.0</td>
      <td>Democratic-Republican</td>
      <td>Lawyer</td>
      <td>Harvard</td>
      <td>32.183908</td>
      <td>NA()</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Andrew Jackson</td>
      <td>8</td>
      <td>1829</td>
      <td>61</td>
      <td>Tennessee</td>
      <td>178</td>
      <td>642553</td>
      <td>1148018</td>
      <td>261</td>
      <td>632.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>None</td>
      <td>68.199234</td>
      <td>55.9706</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Martin Van Buren</td>
      <td>4</td>
      <td>1837</td>
      <td>54</td>
      <td>New York</td>
      <td>170</td>
      <td>764176</td>
      <td>1503534</td>
      <td>294</td>
      <td>429.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>None</td>
      <td>57.823129</td>
      <td>50.8253</td>
    </tr>
    <tr>
      <th>8</th>
      <td>William Henry Harrison</td>
      <td>0.8</td>
      <td>1841</td>
      <td>68</td>
      <td>Ohio</td>
      <td>234</td>
      <td>1275390</td>
      <td>2411808</td>
      <td>294</td>
      <td>329.0</td>
      <td>Whig</td>
      <td>Soldier</td>
      <td>Hampden-Sydney</td>
      <td>79.591837</td>
      <td>52.8811</td>
    </tr>
    <tr>
      <th>9</th>
      <td>James K. Polk</td>
      <td>4</td>
      <td>1845</td>
      <td>49</td>
      <td>Tennessee</td>
      <td>170</td>
      <td>1339494</td>
      <td>2703659</td>
      <td>275</td>
      <td>632.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>U. of North Carolina</td>
      <td>61.818182</td>
      <td>49.5437</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Zachary Taylor</td>
      <td>1</td>
      <td>1849</td>
      <td>64</td>
      <td>Louisiana</td>
      <td>163</td>
      <td>1361393</td>
      <td>2879184</td>
      <td>290</td>
      <td>447.0</td>
      <td>Whig</td>
      <td>Soldier</td>
      <td>None</td>
      <td>56.206897</td>
      <td>47.284</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Franklin Pierce</td>
      <td>4</td>
      <td>1853</td>
      <td>48</td>
      <td>New Hampshire</td>
      <td>254</td>
      <td>1607510</td>
      <td>3161830</td>
      <td>296</td>
      <td>286.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>Bowdoin</td>
      <td>85.810811</td>
      <td>50.8411</td>
    </tr>
    <tr>
      <th>12</th>
      <td>James Buchanan</td>
      <td>4</td>
      <td>1857</td>
      <td>65</td>
      <td>Pennsylvania</td>
      <td>174</td>
      <td>1836072</td>
      <td>4054647</td>
      <td>296</td>
      <td>259.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>Dickinson</td>
      <td>58.783784</td>
      <td>45.2832</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Abraham Lincoln</td>
      <td>4</td>
      <td>1861</td>
      <td>52</td>
      <td>Illinois</td>
      <td>180</td>
      <td>1865908</td>
      <td>4685561</td>
      <td>303</td>
      <td>900.0</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>None</td>
      <td>59.405941</td>
      <td>39.8225</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Ulysses S. Grant</td>
      <td>8</td>
      <td>1869</td>
      <td>46</td>
      <td>Illinois</td>
      <td>214</td>
      <td>3013650</td>
      <td>5722440</td>
      <td>294</td>
      <td>403.0</td>
      <td>Republican</td>
      <td>Soldier</td>
      <td>US Military Academy</td>
      <td>72.789116</td>
      <td>52.6637</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Rutherford B. Hayes</td>
      <td>4</td>
      <td>1877</td>
      <td>54</td>
      <td>Ohio</td>
      <td>185</td>
      <td>4034311</td>
      <td>8413101</td>
      <td>369</td>
      <td>477.0</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>Kenyon</td>
      <td>50.135501</td>
      <td>47.9527</td>
    </tr>
    <tr>
      <th>16</th>
      <td>James A. Garfield</td>
      <td>0.5</td>
      <td>1881</td>
      <td>49</td>
      <td>Ohio</td>
      <td>214</td>
      <td>4446158</td>
      <td>9210420</td>
      <td>369</td>
      <td>444.0</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>Williams</td>
      <td>57.994580</td>
      <td>48.2731</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Grover Cleveland</td>
      <td>4</td>
      <td>1885</td>
      <td>47</td>
      <td>New York</td>
      <td>219</td>
      <td>4874621</td>
      <td>10049754</td>
      <td>401</td>
      <td>576.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>None</td>
      <td>54.613466</td>
      <td>48.5049</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Benjamin Harrison</td>
      <td>4</td>
      <td>1889</td>
      <td>55</td>
      <td>Indiana</td>
      <td>233</td>
      <td>5443892</td>
      <td>11383320</td>
      <td>401</td>
      <td>426.0</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>Miami</td>
      <td>58.104738</td>
      <td>47.8234</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Grover Cleveland</td>
      <td>4</td>
      <td>1893</td>
      <td>55</td>
      <td>New York</td>
      <td>277</td>
      <td>5551883</td>
      <td>12056097</td>
      <td>444</td>
      <td>576.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>None</td>
      <td>62.387387</td>
      <td>46.0504</td>
    </tr>
    <tr>
      <th>20</th>
      <td>William McKinley</td>
      <td>4</td>
      <td>1897</td>
      <td>54</td>
      <td>Ohio</td>
      <td>271</td>
      <td>7108480</td>
      <td>13935738</td>
      <td>447</td>
      <td>601.0</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>Allegheny College</td>
      <td>60.626398</td>
      <td>51.009</td>
    </tr>
    <tr>
      <th>21</th>
      <td>William Howard Taft</td>
      <td>4</td>
      <td>1909</td>
      <td>51</td>
      <td>Ohio</td>
      <td>321</td>
      <td>7676258</td>
      <td>14882734</td>
      <td>483</td>
      <td>491.0</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>Yale</td>
      <td>66.459627</td>
      <td>51.5783</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Woodrow Wilson</td>
      <td>8</td>
      <td>1913</td>
      <td>56</td>
      <td>New Jersey</td>
      <td>435</td>
      <td>6293152</td>
      <td>15040963</td>
      <td>531</td>
      <td>723.0</td>
      <td>Democrat</td>
      <td>Educator</td>
      <td>Princeton</td>
      <td>81.920904</td>
      <td>41.8401</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Warren G. Harding</td>
      <td>2</td>
      <td>1921</td>
      <td>55</td>
      <td>Ohio</td>
      <td>404</td>
      <td>16133314</td>
      <td>26753786</td>
      <td>531</td>
      <td>326.0</td>
      <td>Republican</td>
      <td>Editor</td>
      <td>None</td>
      <td>76.082863</td>
      <td>60.3029</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Herbert Hoover</td>
      <td>4</td>
      <td>1929</td>
      <td>54</td>
      <td>California</td>
      <td>444</td>
      <td>21411991</td>
      <td>36790364</td>
      <td>531</td>
      <td>400.0</td>
      <td>Republican</td>
      <td>Engineer</td>
      <td>Stanford</td>
      <td>83.615819</td>
      <td>58.2</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Franklin Roosevelt</td>
      <td>12</td>
      <td>1933</td>
      <td>51</td>
      <td>New York</td>
      <td>472</td>
      <td>22825016</td>
      <td>39749382</td>
      <td>531</td>
      <td>876.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>Harvard</td>
      <td>88.888889</td>
      <td>57.4223</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Dwight D. Eisenhower</td>
      <td>8</td>
      <td>1953</td>
      <td>62</td>
      <td>New York</td>
      <td>442</td>
      <td>33936137</td>
      <td>61551118</td>
      <td>531</td>
      <td>699.0</td>
      <td>Republican</td>
      <td>Soldier</td>
      <td>US Military Academy</td>
      <td>83.239171</td>
      <td>55.1349</td>
    </tr>
    <tr>
      <th>27</th>
      <td>John F. Kennedy</td>
      <td>3</td>
      <td>1961</td>
      <td>43</td>
      <td>Massachusetts</td>
      <td>303</td>
      <td>34221344</td>
      <td>68828960</td>
      <td>537</td>
      <td>704.0</td>
      <td>Democrat</td>
      <td>Author</td>
      <td>Harvard</td>
      <td>56.424581</td>
      <td>49.7194</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Richard M. Nixon</td>
      <td>5</td>
      <td>1969</td>
      <td>56</td>
      <td>New York</td>
      <td>301</td>
      <td>31785148</td>
      <td>73203370</td>
      <td>538</td>
      <td>477.0</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>Whittier</td>
      <td>55.947955</td>
      <td>43.4203</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Jimmy Carter</td>
      <td>4</td>
      <td>1977</td>
      <td>52</td>
      <td>Georgia</td>
      <td>297</td>
      <td>40830763</td>
      <td>81555889</td>
      <td>538</td>
      <td>518.0</td>
      <td>Democrat</td>
      <td>Businessman</td>
      <td>US Naval Academy</td>
      <td>55.204461</td>
      <td>50.0648</td>
    </tr>
    <tr>
      <th>30</th>
      <td>Ronald Reagan</td>
      <td>8</td>
      <td>1981</td>
      <td>69</td>
      <td>California</td>
      <td>489</td>
      <td>43904153</td>
      <td>86515221</td>
      <td>538</td>
      <td>634.0</td>
      <td>Republican</td>
      <td>Actor</td>
      <td>Eureka College</td>
      <td>90.892193</td>
      <td>50.7473</td>
    </tr>
    <tr>
      <th>31</th>
      <td>George Bush</td>
      <td>4</td>
      <td>1989</td>
      <td>64</td>
      <td>Texas</td>
      <td>426</td>
      <td>48886097</td>
      <td>91584820</td>
      <td>538</td>
      <td>548.0</td>
      <td>Republican</td>
      <td>Businessman</td>
      <td>Yale</td>
      <td>79.182156</td>
      <td>53.3779</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Bill Clinton</td>
      <td>8</td>
      <td>1993</td>
      <td>46</td>
      <td>Arkansas</td>
      <td>370</td>
      <td>44909326</td>
      <td>104425014</td>
      <td>538</td>
      <td>539.0</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>Georgetown</td>
      <td>68.773234</td>
      <td>43.0063</td>
    </tr>
    <tr>
      <th>33</th>
      <td>George W. Bush</td>
      <td>8</td>
      <td>2001</td>
      <td>54</td>
      <td>Texas</td>
      <td>271</td>
      <td>50460110</td>
      <td>105417258</td>
      <td>538</td>
      <td>NaN</td>
      <td>Republican</td>
      <td>Businessman</td>
      <td>Yale</td>
      <td>50.371747</td>
      <td>47.867</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Barack Obama</td>
      <td>n/a</td>
      <td>2009</td>
      <td>47</td>
      <td>Illinois</td>
      <td>365</td>
      <td>69492376</td>
      <td>129438754</td>
      <td>538</td>
      <td>NaN</td>
      <td>Democrat</td>
      <td>Lawyer</td>
      <td>Columbia University</td>
      <td>67.843866</td>
      <td>53.6875</td>
    </tr>
  </tbody>
</table>
</div>



- 웹페이지 표 읽기(행정안전부 지방 물가 정보)

행정안전부 지방물가 정보 사이트 [http://www.mois.go.kr/frt/sub/a02/mulMain/screen.do](http://www.mois.go.kr/frt/sub/a02/mulMain/screen.do)에서 농축산물 전월 평균 가격정보를 가져오자.


```python
import bs4, requests
import pandas as pd

# 행정 안전부 지방 물가 정보 - 농축산물
site = 'http://www.mois.go.kr/frt/sub/a02/farmProductPriceList/screen.do'

resp = requests.get(site)
html = resp.text
bs = bs4.BeautifulSoup(html, 'html.parser')
iframes = bs.select('iframe')
for iframe in iframes:
    frame_site = iframe.attrs['src']
    dfs = pd.read_html(frame_site, na_values=['-'])
df = dfs[0]
print(df)
```

        구분    쇠고기  돼지고기   닭고기    달걀    배추     무    감자  고추가루      콩      쌀
    0   서울   9864  2619  6353  2281  3330  1769  3622  3329  11153  48638
    1   부산   9382  2370  5962  3497  5046  1961  2929  3329   9601  43952
    2   대구   9428  2455  6423  2447  4345  1691  3428  3071   9373  41517
    3   인천   8691  2438  5652  2179  3797  1622  3761  2783   9317  42322
    4   광주  10433  2447  5219  2346  4240  2061  3730  3382   9868  43047
    5   대전   8013  2599  5091  3169  2905  1589  3876  4131   9329  42780
    6   울산   9160  2196  6485  2587  4608  1935  3581  3957  10523  42880
    7   경기   9627  2389  5917  2542  4263  1860  3713  3304   9848  44653
    8   강원   9251  2410  5627  2208  4249  1871  3186  3445   8535  45319
    9   충북   9851  2643  5550  2908  4044  2019  3132  3279   9297  42971
    10  충남   8258  2146  5626  2400  4161  1914  3008  3784   8169  44093
    11  전북   8892  2196  5353  2954  3270  1857  3557  3509   8580  42440
    12  전남   8716  2098  5391  3072  4268  2188  3217  3210   7373  40663
    13  경북   7675  2136  5941  2953  4611  2032  3006  2588   9240  41505
    14  경남   8795  2165  5327  2960  3904  1917  3189  3027   8056  41187
    15  제주   8425  2528  6298  2860  5522  2070  2910  3087   8152  43017
    

pd.read_html('site address')을 이용하여 웹 페이지에 있는 표(table)를 pandas DataFrame 리스트로 변환한다.

- 데이터 프레임 내용 출력


```python
df['구분'] # Series 형으로 출력
```




    0     서울
    1     부산
    2     대구
    3     인천
    4     광주
    5     대전
    6     울산
    7     경기
    8     강원
    9     충북
    10    충남
    11    전북
    12    전남
    13    경북
    14    경남
    15    제주
    Name: 구분, dtype: object




```python
df[['구분', '쇠고기', '감자']] # DataFrame형 출력
```




<div>
<style>
    .dataframe thead tr:only-child th {
        text-align: right;
    }

    .dataframe thead th {
        text-align: left;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>구분</th>
      <th>쇠고기</th>
      <th>감자</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>서울</td>
      <td>9864</td>
      <td>3622</td>
    </tr>
    <tr>
      <th>1</th>
      <td>부산</td>
      <td>9382</td>
      <td>2929</td>
    </tr>
    <tr>
      <th>2</th>
      <td>대구</td>
      <td>9428</td>
      <td>3428</td>
    </tr>
    <tr>
      <th>3</th>
      <td>인천</td>
      <td>8691</td>
      <td>3761</td>
    </tr>
    <tr>
      <th>4</th>
      <td>광주</td>
      <td>10433</td>
      <td>3730</td>
    </tr>
    <tr>
      <th>5</th>
      <td>대전</td>
      <td>8013</td>
      <td>3876</td>
    </tr>
    <tr>
      <th>6</th>
      <td>울산</td>
      <td>9160</td>
      <td>3581</td>
    </tr>
    <tr>
      <th>7</th>
      <td>경기</td>
      <td>9627</td>
      <td>3713</td>
    </tr>
    <tr>
      <th>8</th>
      <td>강원</td>
      <td>9251</td>
      <td>3186</td>
    </tr>
    <tr>
      <th>9</th>
      <td>충북</td>
      <td>9851</td>
      <td>3132</td>
    </tr>
    <tr>
      <th>10</th>
      <td>충남</td>
      <td>8258</td>
      <td>3008</td>
    </tr>
    <tr>
      <th>11</th>
      <td>전북</td>
      <td>8892</td>
      <td>3557</td>
    </tr>
    <tr>
      <th>12</th>
      <td>전남</td>
      <td>8716</td>
      <td>3217</td>
    </tr>
    <tr>
      <th>13</th>
      <td>경북</td>
      <td>7675</td>
      <td>3006</td>
    </tr>
    <tr>
      <th>14</th>
      <td>경남</td>
      <td>8795</td>
      <td>3189</td>
    </tr>
    <tr>
      <th>15</th>
      <td>제주</td>
      <td>8425</td>
      <td>2910</td>
    </tr>
  </tbody>
</table>
</div>



- 값 출력


```python
df_excel['Political Party'].value_counts()
```




    Republican               14
    Democrat                 13
    Democratic-Republican     4
    Whig                      2
    None                      1
    Federalist                1
    Name: Political Party, dtype: int64



#### 기본 통계

- 요약

`describe()` 함수를 이용하여 기본적인 통계량을 관찰할 수 있다. `describe(include='all')`을 이용해서 모든 열에 대해서 통계량을 관찰할 수 있다.


```python
df_excel.describe()
```




<div>
<style>
    .dataframe thead tr:only-child th {
        text-align: right;
    }

    .dataframe thead th {
        text-align: left;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year first inaugurated</th>
      <th>Age at inauguration</th>
      <th># of electoral votes</th>
      <th>Total electoral votes</th>
      <th>Rating points</th>
      <th>% electoral</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>35.000000</td>
      <td>35.000000</td>
      <td>35.000000</td>
      <td>35.000000</td>
      <td>33.000000</td>
      <td>35.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>1892.542857</td>
      <td>55.085714</td>
      <td>261.114286</td>
      <td>385.085714</td>
      <td>552.606061</td>
      <td>68.048420</td>
    </tr>
    <tr>
      <th>std</th>
      <td>64.758530</td>
      <td>6.381828</td>
      <td>118.620198</td>
      <td>143.817567</td>
      <td>159.117280</td>
      <td>15.092928</td>
    </tr>
    <tr>
      <th>min</th>
      <td>1789.000000</td>
      <td>43.000000</td>
      <td>69.000000</td>
      <td>69.000000</td>
      <td>259.000000</td>
      <td>32.183908</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>1843.000000</td>
      <td>51.000000</td>
      <td>176.000000</td>
      <td>292.000000</td>
      <td>444.000000</td>
      <td>57.123855</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>1885.000000</td>
      <td>55.000000</td>
      <td>234.000000</td>
      <td>401.000000</td>
      <td>564.000000</td>
      <td>66.459627</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>1943.000000</td>
      <td>57.500000</td>
      <td>343.000000</td>
      <td>531.000000</td>
      <td>632.000000</td>
      <td>80.756370</td>
    </tr>
    <tr>
      <th>max</th>
      <td>2009.000000</td>
      <td>69.000000</td>
      <td>489.000000</td>
      <td>538.000000</td>
      <td>900.000000</td>
      <td>100.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df_excel.describe(include='all')
```




<div>
<style>
    .dataframe thead tr:only-child th {
        text-align: right;
    }

    .dataframe thead th {
        text-align: left;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>President</th>
      <th>Years in office</th>
      <th>Year first inaugurated</th>
      <th>Age at inauguration</th>
      <th>State elected from</th>
      <th># of electoral votes</th>
      <th># of popular votes</th>
      <th>National total votes</th>
      <th>Total electoral votes</th>
      <th>Rating points</th>
      <th>Political Party</th>
      <th>Occupation</th>
      <th>College</th>
      <th>% electoral</th>
      <th>% popular</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>35</td>
      <td>35.0</td>
      <td>35.000000</td>
      <td>35.000000</td>
      <td>35</td>
      <td>35.000000</td>
      <td>35</td>
      <td>35</td>
      <td>35.000000</td>
      <td>33.000000</td>
      <td>35</td>
      <td>35</td>
      <td>35</td>
      <td>35.000000</td>
      <td>35</td>
    </tr>
    <tr>
      <th>unique</th>
      <td>34</td>
      <td>10.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>15</td>
      <td>NaN</td>
      <td>30</td>
      <td>30</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>6</td>
      <td>10</td>
      <td>20</td>
      <td>NaN</td>
      <td>30</td>
    </tr>
    <tr>
      <th>top</th>
      <td>Grover Cleveland</td>
      <td>4.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Ohio</td>
      <td>NaN</td>
      <td>NA()</td>
      <td>NA()</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Republican</td>
      <td>Lawyer</td>
      <td>None</td>
      <td>NaN</td>
      <td>NA()</td>
    </tr>
    <tr>
      <th>freq</th>
      <td>2</td>
      <td>16.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>6</td>
      <td>NaN</td>
      <td>6</td>
      <td>6</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>14</td>
      <td>21</td>
      <td>8</td>
      <td>NaN</td>
      <td>6</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>1892.542857</td>
      <td>55.085714</td>
      <td>NaN</td>
      <td>261.114286</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>385.085714</td>
      <td>552.606061</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>68.048420</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>std</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>64.758530</td>
      <td>6.381828</td>
      <td>NaN</td>
      <td>118.620198</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>143.817567</td>
      <td>159.117280</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>15.092928</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>min</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>1789.000000</td>
      <td>43.000000</td>
      <td>NaN</td>
      <td>69.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>69.000000</td>
      <td>259.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>32.183908</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>1843.000000</td>
      <td>51.000000</td>
      <td>NaN</td>
      <td>176.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>292.000000</td>
      <td>444.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>57.123855</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>1885.000000</td>
      <td>55.000000</td>
      <td>NaN</td>
      <td>234.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>401.000000</td>
      <td>564.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>66.459627</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>1943.000000</td>
      <td>57.500000</td>
      <td>NaN</td>
      <td>343.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>531.000000</td>
      <td>632.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>80.756370</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>max</th>
      <td>NaN</td>
      <td>NaN</td>
      <td>2009.000000</td>
      <td>69.000000</td>
      <td>NaN</td>
      <td>489.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>538.000000</td>
      <td>900.000000</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>100.000000</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>



- 열별 평균, 합계
`mean()` 함수를 이용하여 평균을 구할 수 있다. 숫자형에 대해서만 계산한다. `sum()`을 이용하여 열별 합계를 구할 수 있다. 문자열일 경우 각 행의 문자열들을 연결한다.


```python
df.mean() # Series형 반환
```




    쇠고기      9028.8125
    돼지고기     2364.6875
    닭고기      5763.4375
    달걀       2710.1875
    배추       4160.1875
    무        1897.2500
    감자       3365.3125
    고추가루     3325.9375
    콩        9150.8750
    쌀       43186.5000
    dtype: float64




```python
df.sum()
```




    구분      서울부산대구인천광주대전울산경기강원충북충남전북전남경북경남제주
    쇠고기                               144461
    돼지고기                               37835
    닭고기                                92215
    달걀                                 43363
    배추                                 66563
    무                                  30356
    감자                                 53845
    고추가루                               53215
    콩                                 146414
    쌀                                 690984
    dtype: object



`df.ix[행슬라이싱, 열슬라이싱]` 을 이용하여 파이썬 슬라이싱 문법을 사용할 수 있다. 또한 이름으로도 가능한다. `df[:, '쇠고기':'닭고기']`를 이용하여 `쇠고기` 열부터 `닭고기` 열까지를 잘라낼 수 있다.


```python
df.iloc[:, 1:].sum()
```




    쇠고기     144461
    돼지고기     37835
    닭고기      92215
    달걀       43363
    배추       66563
    무        30356
    감자       53845
    고추가루     53215
    콩       146414
    쌀       690984
    dtype: int64



- 정렬
`sort_values(by=['colname'])`을 이용해서 지정된 열로 데이터프레임을 정렬할 수 있다.


```python
df.sort_values(by=['쇠고기'])
```




<div>
<style>
    .dataframe thead tr:only-child th {
        text-align: right;
    }

    .dataframe thead th {
        text-align: left;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>구분</th>
      <th>쇠고기</th>
      <th>돼지고기</th>
      <th>닭고기</th>
      <th>달걀</th>
      <th>배추</th>
      <th>무</th>
      <th>감자</th>
      <th>고추가루</th>
      <th>콩</th>
      <th>쌀</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>13</th>
      <td>경북</td>
      <td>7675</td>
      <td>2136</td>
      <td>5941</td>
      <td>2953</td>
      <td>4611</td>
      <td>2032</td>
      <td>3006</td>
      <td>2588</td>
      <td>9240</td>
      <td>41505</td>
    </tr>
    <tr>
      <th>5</th>
      <td>대전</td>
      <td>8013</td>
      <td>2599</td>
      <td>5091</td>
      <td>3169</td>
      <td>2905</td>
      <td>1589</td>
      <td>3876</td>
      <td>4131</td>
      <td>9329</td>
      <td>42780</td>
    </tr>
    <tr>
      <th>10</th>
      <td>충남</td>
      <td>8258</td>
      <td>2146</td>
      <td>5626</td>
      <td>2400</td>
      <td>4161</td>
      <td>1914</td>
      <td>3008</td>
      <td>3784</td>
      <td>8169</td>
      <td>44093</td>
    </tr>
    <tr>
      <th>15</th>
      <td>제주</td>
      <td>8425</td>
      <td>2528</td>
      <td>6298</td>
      <td>2860</td>
      <td>5522</td>
      <td>2070</td>
      <td>2910</td>
      <td>3087</td>
      <td>8152</td>
      <td>43017</td>
    </tr>
    <tr>
      <th>3</th>
      <td>인천</td>
      <td>8691</td>
      <td>2438</td>
      <td>5652</td>
      <td>2179</td>
      <td>3797</td>
      <td>1622</td>
      <td>3761</td>
      <td>2783</td>
      <td>9317</td>
      <td>42322</td>
    </tr>
    <tr>
      <th>12</th>
      <td>전남</td>
      <td>8716</td>
      <td>2098</td>
      <td>5391</td>
      <td>3072</td>
      <td>4268</td>
      <td>2188</td>
      <td>3217</td>
      <td>3210</td>
      <td>7373</td>
      <td>40663</td>
    </tr>
    <tr>
      <th>14</th>
      <td>경남</td>
      <td>8795</td>
      <td>2165</td>
      <td>5327</td>
      <td>2960</td>
      <td>3904</td>
      <td>1917</td>
      <td>3189</td>
      <td>3027</td>
      <td>8056</td>
      <td>41187</td>
    </tr>
    <tr>
      <th>11</th>
      <td>전북</td>
      <td>8892</td>
      <td>2196</td>
      <td>5353</td>
      <td>2954</td>
      <td>3270</td>
      <td>1857</td>
      <td>3557</td>
      <td>3509</td>
      <td>8580</td>
      <td>42440</td>
    </tr>
    <tr>
      <th>6</th>
      <td>울산</td>
      <td>9160</td>
      <td>2196</td>
      <td>6485</td>
      <td>2587</td>
      <td>4608</td>
      <td>1935</td>
      <td>3581</td>
      <td>3957</td>
      <td>10523</td>
      <td>42880</td>
    </tr>
    <tr>
      <th>8</th>
      <td>강원</td>
      <td>9251</td>
      <td>2410</td>
      <td>5627</td>
      <td>2208</td>
      <td>4249</td>
      <td>1871</td>
      <td>3186</td>
      <td>3445</td>
      <td>8535</td>
      <td>45319</td>
    </tr>
    <tr>
      <th>1</th>
      <td>부산</td>
      <td>9382</td>
      <td>2370</td>
      <td>5962</td>
      <td>3497</td>
      <td>5046</td>
      <td>1961</td>
      <td>2929</td>
      <td>3329</td>
      <td>9601</td>
      <td>43952</td>
    </tr>
    <tr>
      <th>2</th>
      <td>대구</td>
      <td>9428</td>
      <td>2455</td>
      <td>6423</td>
      <td>2447</td>
      <td>4345</td>
      <td>1691</td>
      <td>3428</td>
      <td>3071</td>
      <td>9373</td>
      <td>41517</td>
    </tr>
    <tr>
      <th>7</th>
      <td>경기</td>
      <td>9627</td>
      <td>2389</td>
      <td>5917</td>
      <td>2542</td>
      <td>4263</td>
      <td>1860</td>
      <td>3713</td>
      <td>3304</td>
      <td>9848</td>
      <td>44653</td>
    </tr>
    <tr>
      <th>9</th>
      <td>충북</td>
      <td>9851</td>
      <td>2643</td>
      <td>5550</td>
      <td>2908</td>
      <td>4044</td>
      <td>2019</td>
      <td>3132</td>
      <td>3279</td>
      <td>9297</td>
      <td>42971</td>
    </tr>
    <tr>
      <th>0</th>
      <td>서울</td>
      <td>9864</td>
      <td>2619</td>
      <td>6353</td>
      <td>2281</td>
      <td>3330</td>
      <td>1769</td>
      <td>3622</td>
      <td>3329</td>
      <td>11153</td>
      <td>48638</td>
    </tr>
    <tr>
      <th>4</th>
      <td>광주</td>
      <td>10433</td>
      <td>2447</td>
      <td>5219</td>
      <td>2346</td>
      <td>4240</td>
      <td>2061</td>
      <td>3730</td>
      <td>3382</td>
      <td>9868</td>
      <td>43047</td>
    </tr>
  </tbody>
</table>
</div>



## 시각화


```python
get_ipython().magic('matplotlib inline')
import matplotlib.pyplot as plt
import numpy as np
from matplotlib import font_manager, rc

font_name = font_manager.FontProperties(fname="c:/Windows/Fonts/malgun.ttf").get_name()
rc('font', family=font_name)
```

- line


```python
import numpy as np

df.set_index('구분').plot(kind='line', xticks=np.arange(len(df['구분'])), rot=90)
```




    <matplotlib.axes._subplots.AxesSubplot at 0x1d0f8b1d0b8>




![png](images/output_34_1.png)


`xticks=np.arange(16)`는 xtick이 보여질 위치를 지정하는 것이다.

- boxplot


```python
df.boxplot()
```




    <matplotlib.axes._subplots.AxesSubplot at 0x1d0fc939e10>




![png](images/output_36_1.png)


- 파이 그래프


```python
df_excel['Political Party'].value_counts().plot(kind="pie")
```




    <matplotlib.axes._subplots.AxesSubplot at 0x1d0fcc60908>




![png](images/output_38_1.png)


- 바차트


```python
df_excel['Political Party'].value_counts().plot(kind="bar")
```




    <matplotlib.axes._subplots.AxesSubplot at 0x1d0fd1f2780>




![png](images/output_40_1.png)


## 참고 사이트

- Beautiful Soup: https://www.crummy.com/software/BeautifulSoup/bs4/doc/#
- requests: http://pythonstudy.xyz/python/article/403-%ED%8C%8C%EC%9D%B4%EC%8D%AC-Web-Scraping
- urllib: https://www.acmicpc.net/blog/view/16
- Python for Data Analysis by Wes McKinney: https://github.com/wesm/pydata-book
- http://www.hanbit.co.kr/channel/category/category_view.html?cms_code=CMS9481416663
- Python for Data Analysis by Wes McKinney: https://github.com/wesm/pydata-book
- Pandas Documentation: http://pandas.pydata.org/pandas-docs/stable/

# 영상 데이터
## 참고 사이트
- 파이썬 이미지 처리 블로그: http://pythonstudy.xyz/python/article/406-%ED%8C%8C%EC%9D%B4%EC%8D%AC-%EC%9D%B4%EB%AF%B8%EC%A7%80-%EC%B2%98%EB%A6%AC
- Pillow documentation: https://pillow.readthedocs.io/en/4.2.x/

## 소개

이미지를 저장하는 형식은 jpg, png, tif, gif등 여러 가지가 있다. 이미지는 픽셀(화소)로 구성된다. 다음 설명은 파이썬 모듈 `Pillow`에서 사용되는 형식이다. 이미지를 다루는 도구마다 약간씩 차이가 있다.

### 크기와 좌표(coordinate system)

- 이미지의 크기는 너비(또는 가로, width), 높이(또는 세로, height)로 구성된다. 너비와 높이는 픽셀의 갯수로 결정된다.
- 픽셀은 2차원 좌표로 표현할 수 있다. 이미지의 왼쪽 위가 (0,0)이고, 각 픽셀은 좌표 (x, y)로 나타낸다. 첫번째 성분 x는 너비를 나타내고 두번째 성분 y는 높이를 나타낸다. x는 왼쪽에서 오른쪽으로 증가하고, y는 위에서 아래로 증가한다.
- 이미지의 부분을 표현하기 위해서 사각형을 이용한다. 사각형은 (x, y, z, w)로 표현하며 x, y는 각각 부분 이미지의 왼쪽, 위의 좌표를 나타내고, z, w는 각각 부분 이미지의 오른쪽, 아래의 좌표를 나타낸다. z, w는 포함되지 않는다. (0, 0, 800, 600)은 800x600 크기를 표현한다.

### 모드(mode)
모드는 픽셀값을 구성하는 방법이다.

- 이진 영상(binary image)는 픽셀이 1 비트로 구성되어 있어서 검은색은 0, 흰색은 1로 표현한다.
- 흑백 영상(gray-scale image) 흑백의 표현을 0 - 255의 숫자로 표현한다. 가장 어두운 것은 0, 가장 밝은 것은 255로 표현한다. 하나의 픽셀을 표현하기 위해 8비트가 사용된다.
- 컬러 영상(color image)은 하나의 픽셀을 표현하기 위해서 3개의 색 빨간(R), 초록(G), 파란(B)색을 사용한다. 각각의 R, G, B는 8비트로 이루어져 있으며 0 - 255의 숫자로 표현한다. 숫자가 커지면 각각의 색이 짙어진다. 빚의 삼원색 원리가 적용되어 (255, 255, 255)는 흰색을 나타내고 (0, 0, 0)은 검은색을 나타낸다. 뿐만 아니라 투명도를 표현하기 위해서 Alpha 채널을 추가하여, (R, G, B, A) 4개의 채널을 사용하기도 한다. alpha 채널에서 0는 투명, 255는 불투명을 의미한다. 이외에도 HSV(Hue, Saturation, Intensity), CMYK, YCbCr 모델등 여러 가지가 있다.

### 밴드(band)
밴드 또는 채널(channel)이라고 하며 픽셀을 구성하는 방법으로 흑백은 1 채널을 가지고 있고 컬러 영상은 R, G, B 3개의 채널(밴드)를 가지고 있다. 또는 R, G, B, A이면 4개의 밴드를 가지고 있다.

## 준비

이미지 처리를 하기 위한 모듈 `Pillow`를 설치한다.

```python
pip install Pillow
```

우선 이미지를 웹사이트에서 다운받아 images폴더를 만들고 그 안에 저장한다.


```python
import requests
import os
from io import BytesIO
from PIL import Image

dir = 'images'
if not os.path.exists(dir):
    os.makedirs(dir)

url = 'https://upload.wikimedia.org/wikipedia/en/2/24/Lenna.png'
response = requests.get(url)
img = Image.open(BytesIO(response.content))

img.save('images/lenna.png')

logo_url = 'https://upload.wikimedia.org/wikipedia/commons/thumb/0/0a/Python.svg/48px-Python.svg.png'
response = requests.get(logo_url)
logo_img = Image.open(BytesIO(response.content))

logo_img.save('images/logo.png')

jisung_url = 'http://i.imgur.com/pbgsMRV.jpg'
response = requests.get(jisung_url)
jisung_img = Image.open(BytesIO(response.content))

jisung_img.save('images/jisung.png')
```

## 읽기/쓰기


```python
from PIL import Image
import matplotlib.pyplot as plt

# 이미지 열기
img = Image.open('images/lenna.png')
 
# 이미지 크기 출력
print(img.format, img.size, img.mode)

# 이미지 보기
plt.imshow(img)

# 이미지 JPG로 저장
img.save('images/lenna.jpg')
```

    PNG (512, 512) RGB
    


![png](images/output_45_1.png)



```python
# Thumbnail 이미지 생성
size = (128, 128)
img.thumbnail(size)  
 
img.save('images/lenna-thumb.jpg')
```

## 잘라내기/붙이기

- 잘라내기

사각형 (left, upper, right, lower)을 이용해서 이미지의 부분을 잘라낼 수 있다.


```python
img = Image.open('images/lenna.png')
box = (100, 100, 400, 400)
cropImage = img.crop(box)
cropImage.save('images/lenna-crop.jpg')
plt.imshow(cropImage)
cropImage.show() # 윈도우즈 기본 그림 보기 프로그램 실행
```


![png](images/output_48_0.png)


- 붙이기

`paste(region, box)`를 이용해서 `region`이미지를 직사각형 `box` 위치에 붙여 넣을 수 있다. `region`의 크기와 `box`의 크기가 같아야 한다.


```python
img1 = img.copy()
box = (50, 50, 350, 350)
cropImage = img1.crop(box)
region = cropImage.rotate(180)
img1.paste(region, box)
plt.axis("off")
plt.imshow(img1)
```




    <matplotlib.image.AxesImage at 0x1d0fd3670f0>




![png](images/output_50_1.png)


- 파이썬 로고 붙이기


```python
img = Image.open('images/lenna.png')
logo = Image.open('images/logo.png')
img1 = img.copy()
position = ((img1.width - logo.width), (img1.height - logo.height))
# img1.paste(logo, position)
img1.paste(logo, position, logo)
img1.save('images/lenna-logo.jpg')
```

paste 함수의 3번째 인수는 mask이고 mask가 될 수 있는 이미지의 모드는 '1'(이진 영상), 'L'(8비트 흑백 영상), 'RGBA'이다. 'RGBA' 영상을 사용하면 alpha 채널의 값을 mask로 사용하게 된다. 알파 채널에서 0은 투명을 의미하고 255는 불투명을 의미한다.


```python
print("logo의 모드:", logo.mode, "(0,0)에서의 픽셀(r,g,b,a):", logo.getpixel((0,0)))
```

    logo의 모드: RGBA (0,0)에서의 픽셀(r,g,b,a): (0, 0, 0, 0)
    

`logo` 이미지의 픽셀 (0,0) 위치에서 alpha 밴드의 값이 0(투명)이므로, 기존 이미지 `lenna.png`의 픽셀을 그대로 보여주게 된다.

## 회전 및 크기 변경


```python
from PIL import Image
img = Image.open('images/lenna.png')
 
# 크기를 600x600 으로
img2 = img.resize((600, 600))
img2.save('images/lenna-600.jpg')
 
# 시계 반대 방향으로 90도 회전
img3 = img.rotate(90)
img3.save('images/lenna-rotate.jpg')

plt.imshow(img3)
```




    <matplotlib.image.AxesImage at 0x1d0fd63d6a0>




![png](images/output_56_1.png)



```python
img4 = img.rotate(18)
plt.imshow(img4)
```




    <matplotlib.image.AxesImage at 0x1d0fd6956d8>




![png](images/output_57_1.png)


`expand=True` 선택을 하면 전체 그림이 보이며 새로 만들어진 이미지의 크기는 증가한다.


```python
img5 = img.rotate(18, expand=True)
plt.imshow(img5)
```




    <matplotlib.image.AxesImage at 0x1d0fd9b04a8>




![png](images/output_59_1.png)


## 필터링

`filter()` 함수와 BLUR, CONTOUR, DETAIL, EDGE_ENHANCE, EDGE_ENHANCE_MORE, EMBOSS, FIND_EDGES, SMOOTH, SMOOTH_MORE, SHARPEN등의 필터들을 사용하여 이미지를 변형한다.

- 블러링


```python
from PIL import Image, ImageFilter
 
img = Image.open('images/lenna.png')
blurImage = img.filter(ImageFilter.BLUR)
 
blurImage.save('images/lenna-blur.png')
```

`transpose(method)` 함수와 method 인자을 이용하여 이미지를 변형할 수 있다. method가 될 수 있는 것은PIL.Image.FLIP_LEFT_RIGHT, PIL.Image.FLIP_TOP_BOTTOM, PIL.Image.ROTATE_90, PIL.Image.ROTATE_180, PIL.Image.ROTATE_270 or PIL.Image.TRANSPOSE이 있다.


```python
img = Image.open('images/lenna.png')
flipImage = img.transpose(Image.FLIP_LEFT_RIGHT)
 
plt.imshow(flipImage)
```




    <matplotlib.image.AxesImage at 0x1d0feb28ac8>




![png](images/output_63_1.png)


## 점(픽셀) 연산
`point()` 함수를 이용하여 각 픽셀에 대한 연산을 수행하여 픽셀의 값을 변경할 수 있다.


```python
# multiply each pixel by 1.2, 전체적으로 이미지가 밝아지는 효과
out = img.point(lambda i: i * 1.2)
plt.imshow(out)
```




    <matplotlib.image.AxesImage at 0x1d0fd1f8898>




![png](images/output_65_1.png)


- 채널에 대한 연산을 수행


```python
# split the image into individual bands
source = img.split()

R, G, B = 0, 1, 2

# 빨간색이 100 보다 크면 255, 그렇지 않으면 0
mask = source[R].point(lambda i: i > 100 and 255)

# 녹색 채널의 값을 줄인다.
out = source[G].point(lambda i: i * 0.7)

# paste the processed band back, but only where red was < 100
source[G].paste(out, None, mask)

# build a new multiband image
img1 = Image.merge(img.mode, source)

plt.imshow(img1)
```




    <matplotlib.image.AxesImage at 0x1d0fd19ddd8>




![png](images/output_67_1.png)


`x and y` 연산은 x가 거짓(0)이면 결과값은 x(0)이고 참이면 결과값은 y가 된다.

# 얼굴 인식

## 준비

### opencv설치

아나콘다 명령어창에서 다음과 같이 입력한다.

```python
conda install -c conda-forge opencv # opencv 3.3, 아나콘다
```

### xml 파일들 다운로드


```python
import urllib.request
import os

directory = 'xmls'
if not os.path.exists(directory):
    os.makedirs(directory)

files = ['haarcascade_frontalface_default.xml',
         'haarcascade_eye.xml']

for file in files:
    url = 'https://raw.githubusercontent.com/opencv/opencv/master/data/haarcascades/' + file
    fpath = directory + '/' + file
    if not os.path.exists(fpath):
        urllib.request.urlretrieve(url, fpath)
```

## 사진

- opencv 이용

```python
import numpy as np
import cv2

face_cascade = cv2.CascadeClassifier('xmls/haarcascade_frontalface_default.xml')
eye_casecade = cv2.CascadeClassifier('xmls/haarcascade_eye.xml')

img = cv2.imread('images/jisung.png')

# 컬러를 회색 영상으로 변환
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

# scaleFactor = 1.1은 0.1 * 100 % = 10 %로 그림을 줄여 나가면서 얼굴을 찾는다.
# 숫자가 작으면 더 정확하게 얼굴들을 찾아내지만 시간이 많이 걸리고 또한 얼굴이 아닌 것을 찾을 가능성이 커진다.
# scaleFactor는 1보다 커야 한다.
# minNeighbors = 5는 후보가 되는 사각형을 적어도 5개의 사각형들이 포함하고 있어야 한다는 것이다.
#  갯수가 많아지면 더 정확한 얼굴을 찾지만 그만큼 원하는 얼굴들을 찾지 못할 수 있다.
# 탐색된 얼굴에 대한 직사각형 리스트 반환
faces = face_cascade.detectMultiScale(gray, 1.1, 5)

for (x, y, w, h) in faces:
    # 이미지에 탐색된 얼굴 직사각형 표시
    # 두번째 인자 (x, y)는 직사각형의 왼쪽 위, 3번째 인자 (x+w, y+h)는 직사각형의 오른쪽 아래,
    # 4번째 인자 (255, 0, 0)는 직사각형 색,
    # 다섯번째 인자 2는 직사각형 둘레의 두께
    cv2.rectangle(img, (x, y), (x+w, y+h), (255, 0, 0), 2)
    # 탐색된 얼굴부분만 변수로 저장
    roi_gray = gray[y:y+h, x:x+w]
    roi_color = img[y:y+h, x:x+w]

    # 얼굴 부분에서 눈 탐색
    eyes = eye_casecade.detectMultiScale(roi_gray)
    for (ex, ey, ew, eh) in eyes:
        # 탐색된 얼굴 부분에 탐색된 눈 부분 직사각형 표시
        cv2.rectangle(roi_color, (ex, ey), (ex+ew, ey+eh), (0, 255, 0), 2)

cv2.imshow('Face Detection', img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## 비디오

- 얼굴 인식

```python
import cv2
import sys
import datetime as dt
from time import sleep

cascPath = "xmls/haarcascade_frontalface_default.xml"
faceCascade = cv2.CascadeClassifier(cascPath)

video_capture = cv2.VideoCapture(0)
anterior = 0

while True:
    if not video_capture.isOpened():
        print('Unable to load camera.')
        sleep(5)
        pass

    # Capture frame-by-frame
    ret, frame = video_capture.read()

    gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

    faces = faceCascade.detectMultiScale(
        gray,
        scaleFactor=1.1,
        minNeighbors=5,
        minSize=(30, 30)
    )

    # Draw a rectangle around the faces
    for (x, y, w, h) in faces:
        cv2.rectangle(frame, (x, y), (x+w, y+h), (0, 255, 0), 2)

    if anterior != len(faces):
        anterior = len(faces)

    # Display the resulting frame
    cv2.imshow('Video', frame)


    if cv2.waitKey(1) & 0xFF == ord('q'):
        break

# When everything is done, release the capture
video_capture.release()
cv2.destroyAllWindows()
```

## 참고 사이트

- OpenCV 얼굴 인식: https://docs.opencv.org/3.3.0/d7/d8b/tutorial_py_face_detection.html
- dlib 얼굴 인식 예제 코드: http://dlib.net/face_recognition.py.html
- https://realpython.com/blog/python/face-detection-in-python-using-a-webcam/
- https://github.com/shantnu/Webcam-Face-Detect

# 사물인식(object detection)

## 필요한 모듈 설치

`imutils` 모듈 설치 필요

```python
pip install imutils
```

## 모델 다운로드

```python
import urllib.request
import os

files = ['MobileNetSSD_deploy.caffemodel',
         'MobileNetSSD_deploy.prototxt.txt']

urls = ['http://gofile.me/6w7gF/egVdflHDS', 'http://gofile.me/6w7gF/dr7GO5SBS']

for (url, file) in zip(urls, files):
    print(url, file)
    if not os.path.exists(file):
        urllib.request.urlretrieve(url, file)
```

### 실행

아래 코드를 `real_time_object_detection.py` 이름으로 저장한다.

```python
# USAGE
# python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel

# import the necessary packages
from imutils.video import VideoStream
from imutils.video import FPS
import numpy as np
import argparse
import imutils
import time
import cv2

# construct the argument parse and parse the arguments
ap = argparse.ArgumentParser()
ap.add_argument("-p", "--prototxt", required=True,
	help="path to Caffe 'deploy' prototxt file")
ap.add_argument("-m", "--model", required=True,
	help="path to Caffe pre-trained model")
ap.add_argument("-c", "--confidence", type=float, default=0.2,
	help="minimum probability to filter weak detections")
args = vars(ap.parse_args())

# initialize the list of class labels MobileNet SSD was trained to
# detect, then generate a set of bounding box colors for each class
CLASSES = ["background", "aeroplane", "bicycle", "bird", "boat",
	"bottle", "bus", "car", "cat", "chair", "cow", "diningtable",
	"dog", "horse", "motorbike", "person", "pottedplant", "sheep",
	"sofa", "train", "tvmonitor"]
COLORS = np.random.uniform(0, 255, size=(len(CLASSES), 3))

# load our serialized model from disk
print("[INFO] loading model...")
net = cv2.dnn.readNetFromCaffe(args["prototxt"], args["model"])

# initialize the video stream, allow the cammera sensor to warmup,
# and initialize the FPS counter
print("[INFO] starting video stream...")
vs = VideoStream(src=0).start()
time.sleep(2.0)
fps = FPS().start()

# loop over the frames from the video stream
while True:
	# grab the frame from the threaded video stream and resize it
	# to have a maximum width of 400 pixels
	frame = vs.read()
	frame = imutils.resize(frame, width=400)

	# grab the frame dimensions and convert it to a blob
	(h, w) = frame.shape[:2]
	blob = cv2.dnn.blobFromImage(cv2.resize(frame, (300, 300)),
		0.007843, (300, 300), 127.5)

	# pass the blob through the network and obtain the detections and
	# predictions
	net.setInput(blob)
	detections = net.forward()

	# loop over the detections
	for i in np.arange(0, detections.shape[2]):
		# extract the confidence (i.e., probability) associated with
		# the prediction
		confidence = detections[0, 0, i, 2]

		# filter out weak detections by ensuring the `confidence` is
		# greater than the minimum confidence
		if confidence > args["confidence"]:
			# extract the index of the class label from the
			# `detections`, then compute the (x, y)-coordinates of
			# the bounding box for the object
			idx = int(detections[0, 0, i, 1])
			box = detections[0, 0, i, 3:7] * np.array([w, h, w, h])
			(startX, startY, endX, endY) = box.astype("int")

			# draw the prediction on the frame
			label = "{}: {:.2f}%".format(CLASSES[idx],
				confidence * 100)
			cv2.rectangle(frame, (startX, startY), (endX, endY),
				COLORS[idx], 2)
			y = startY - 15 if startY - 15 > 15 else startY + 15
			cv2.putText(frame, label, (startX, y),
				cv2.FONT_HERSHEY_SIMPLEX, 0.5, COLORS[idx], 2)

	# show the output frame
	cv2.imshow("Frame", frame)
	key = cv2.waitKey(1) & 0xFF

	# if the `q` key was pressed, break from the loop
	if key == ord("q"):
		break

	# update the FPS counter
	fps.update()

# stop the timer and display FPS information
fps.stop()
print("[INFO] elapsed time: {:.2f}".format(fps.elapsed()))
print("[INFO] approx. FPS: {:.2f}".format(fps.fps()))

# do a bit of cleanup
cv2.destroyAllWindows()
vs.stop()
```

아나콘다 프롬프트 창에서 아래와 같이 입력한다.

```python
python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel
```

`q`를 눌러서 종료할 수 있는데 종료가 안될 경우도 생긴다. 그럴때는 ctrl + alt + del을 눌러서 연결된 python 실행을 강제로 종료해야 한다.


### 참고 사이트

- https://realpython.com/blog/python/face-detection-in-python-using-a-webcam/
- https://github.com/shantnu/Webcam-Face-Detect
- https://www.pyimagesearch.com/2017/09/18/real-time-object-detection-with-deep-learning-and-opencv/
- MobileNet-SSD 탐색 네트워크 카페 구현: https://github.com/chuanqi305/MobileNet-SSD
