# MySql

## MySql 설치방법

* 구글창에 bitnami wamp 검색 후 나오는 웹사이트 누름 (윈도우에서 Apache, MySql, PHP 동시에 설치하게 해주는 프로그램)
* 최신버전으로 다운로드
* 다운받고 셋업할 때 root(기본) 사용자의 비밀번호를 설정해주어야함
* 다운로드가 완료되면 Bitnami WAMP stack manager tool이 실행됨
* Manage Server 탭으로 가면 MySql Database가 실행중인지 나오고 실행중이아니면 Start를 누르면 됨
* 이 프로그램이 깔려있는 위치는 C드라이브의 Bitnami디렉토리에 깔려있음 manager-windows 아이콘을 누르면 실행됨

## 커맨드프롬프트로 MySql 실행방법

* 윈도우 + r 키를누르고 cmd를 입력
* 프롬프트 창에서 cd C:\Bitnami\wampstack...\mysql\bin 입력
* 다시 mysql -uroot -p 입력
* 그럼 패스워드를 입력하라고 나오는데, 설치시 설정한 패스워드를 입력하면 Welcome to the MySQL monitor 라고 나옴.
* 그럼 mysql> 로 시작하는 부분에서 sql명령어를 입력하여 작업을 진행할 수 있음.

## Workbench 설치방법

* MySQL Workbench를 구글창에 타입 후 웹사이트 접속
* 화면에 바로 나오는 Download Now 클릭
* Operating System 설정 후 다운로드
* 만일 Visual C++ Redistributable 2019 에러가 뜨면, [https://www.itechtics.com/microsoft-visual-c-redistributable-versions-direct-download-links/#6-microsoft-visual-c-redistributable-2019](https://www.itechtics.com/microsoft-visual-c-redistributable-versions-direct-download-links/#6-microsoft-visual-c-redistributable-2019)다운로드
* 그 후 다시 workbench를 다운로드하면 됨

## Workbench 초기실행방법

* MySQL Connection 옆에 +버튼을 누름
* Connection Name 설정
* Connection Method 스탠다드
* Hostname 127.0.0.1
* Port 3306
* Username 설정
* Test Connection을 누르면 초기에 설정해둔 비밀번호를 입력하라고 나옴
* 입력 후 OK 누르면 새로운 커넥션이 생성됨

## 워크벤치에서 새로운 스키마를 만드는 방법

* Create a new schema in the connected server 버튼을 클릭
* 뜨는 화면에 새로운 schema name을 입력
* Apply를 클릭
* 클릭하면 바로 실행되는 것이아니라 지금 하려는 일에 해당되는 SQL문이 뜸
* 다시 Apply를 누르면 실행이 됨
* 잘 실행 되었는지 프롬프트에서 확인하는 법은 SHOW DATABASES; 를 커맨드 프롬프트에 입력하면 데이터베이스안의 스키마들이 보여짐

## 워크벤치에서 새로운 테이블을 만드는 방법

* Create a new table in the active schema을 클릭. 테이블을 만드는데 지금 활성화되어있는 스키마안에서 만듬
* 테이블 네임을 지정해줌
* 그 후, 예를들어 컬럼에 id, datatype, PK(primary key), NN(not null), AI(auto-increment)등을 지정해주면서 칼럼을 추가함
* 그 후, Apply를 누르면 SQL문이 다시 나옴
* 다시 Apply를 누르면 실행됨
* 확인하려면 Tables를 누르면 됨
* Tables 밑에 새로생성된 테이블이 있을 것임

## Workbench에서 csv파일을 import하는법

* 스키마에 새로운 테이블을 만들고 칼럼네임들을 csv파일의 칼럼네임과 같게 만든다
* csv파일의 칼럼네임이 쓰여져있는 첫 행을 지운다
* ![image1.png](/https://github.com/Taeheonic/Data-Science/img/image1.png)
* ![image2.png](/https://github.com/Taeheonic/Data-Science/img/image2.png)
* 테이블이 만들어진 것을 확인할 수 있음

## 명령 프롬프트를 이용하여 csv파일을 import하는법
