# TIL

# ChatGPT

## GPT란 무엇인가?

- G : Generative (생성적인) → 주어진 입력에 기반하여 새로운 데이터를 생성
- P : Pre-Traimed (미리 학습된)
- T : Transformer (어텐션 메커니즘) → 자연어 처리작업에 사용되는 딥러닝 모델
- 단점 : 말도 안되는 질문을 해도 말이 되게 지어내서 설명한다 → 신뢰도가 100퍼가 아니다.

## API (Application Programming Interface)

- 두 소프트웨어가 서로 통신할 수 있게 하는 메커니즘
- **두 소프트웨어 : Client, Server**
- Client ↔ Server ↔ Database
    - Client는 Server에게 ‘요청’ 하고,
    - Server는 Client에게 ‘응답’ 한다.
- 통신 : 데이터를 주고 받는 것
- API Key : Client가 Server에게 데이터를 요청하는 수단 (완전한 정의는 아님)
    - API는 Server 개발자가 정하고, 배포한다.
    - Client 요청 (API) ↔ 서버 응답 (JSON) 형태로 상호작용함
- Interface = TV의 리모컨과 같다
- UI : 사용자와 소프트웨어 간의 상호작용 시스템

## 프론트의 구성

**HTML (HyperText Markup Language)은 웹 페이지의 뼈대**를 구성하는 언어입니다. HTML은 웹 페이지의 구조와 내용을 정의하며, 텍스트, 이미지, 링크 등을 포함할 수 있습니다.

**CSS (Cascading Style Sheets)는 웹 페이지의 디자인과 스타일**을 담당하는 언어입니다. CSS를 사용하여 HTML 요소의 색상, 크기, 배치 등을 지정할 수 있습니다. CSS는 웹 페이지를 더욱 시각적으로 표현하고 사용자 경험을 개선하는 데 사용됩니다.

**JS (JavaScript)는 웹 페이지에 동적인 기능**을 추가하기 위해 사용되는 프로그래밍 언어입니다. JS를 사용하여 사용자와의 상호작용이 가능한 웹 페이지를 만들 수 있으며, 데이터의 처리와 조작, 이벤트 처리, 애니메이션 등을 구현할 수 있습니다.

- HTML : 뼈대
- CSS : 디자인과 스타일
- JS : 동적인 기능


# 트랙 특화 2일차 시작

- MarkDown
- CLI
- GIT
- HTML : HyperText Markup Language의 약자
- Markdown : 마크업 언어
    - Git에선 작성 필수는 아니다.
    - 주로 개발자들이 텍스트와 코드를 작성해 문서화하기 위해 사용
    - 작성된 markdown 문서는 다른 프로그램에 의해 변환되어 출력됨

## 마크 다운

- 진행 상황
    - touch README.md
    - extension → markdown all in one 설치
    - 오른쪽 클릭 → open preview 또는 open preview to side 기능을 통해 미리 볼 수 있다.
    - **md의 기능? 외울 필요 없다! → Why? 마크 다운에도 공식 문서가 존재한다!!**
        
        [Basic Syntax | Markdown Guide](https://www.markdownguide.org/basic-syntax/)
        
    - 반드시 기능 뒤에 ‘공백’을 넣어야 기능이 적용된다!!
    - **강사님에게 코딩관련 질문을 할 시, ‘코드 블럭’ 기능을 이용해주면 좋다.**
    - 이미지 걸기 기능
        - 그냥 이미지 주소 복사하고 붙이면 너무 길게 작성됨
        - 바로 붙여넣기 하지말고 사이트 들어가서 주소를 가져오면 짧게 되는 경우가 있음
        - 너무 길면 가독성이 떨어지니 메모장에 복붙 후 길이를 보고 결정하도록 하자
        - **마크 다운 이미지에서는 정렬을 하거나 배치를 바꿀 수 없다.**
    - 굵은 글씨
        - 중간에 넣을 때는 ** 굵은 ** 방식을 사용해야 한다.

## 인터페이스 방식

- 대상을 제어하는 방법, 수단 (ex TV 제어 하는 방법 → 리모컨)
- GUI ↔ CLI (TUI는 최근 사용하지 않는다)
    - Windows OS  CLI : Power Shell, cmd
    - Linux OS CLI : Bash  ← bash에서 git 사용을 주로 많이 씀 → ‘git bash’ 라고 부른다
- Git을 다룰 때 interface
    - GUI : Github Desktop(기능이 적음)
        - 장점 : 보기 편함, 친숙함, 기능 다있음
        - **최고 장점 : Graph를 훨씬 보기 좋다, diff 파일 비교 → 복잡한 분석은 GUI가 좋다!!**
        - 아틀라시안 제품인 ‘소스트리’를 많이 사용함 → 최고!
    - CLI : Git bash
        - 장점: Commit, Push 명령어 1초면 사용 종료. (GUI는 비교적 오래걸림)
        - 20년 전에 쓰는 것을 지금도 사용중이고, 앞으로도 사용할 예정이다. (바뀔 일이 없다)
- **결론 - 대부분 CLI를 쓰지만, diff 나 graph는 GUI를 쓸 예정이다.**

## Git Bash 실습

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/11c46b42-5382-4dc7-961e-be37754766c7/9193e872-07f9-4ad8-84ec-bfc50335db50/Untitled.png)

- 초록색 → PC 환경
- 보라색 : MINGW64
    - MinGW64는 Windows 운영 체제에서 실행할 수 있는 GNU 도구 모음의 64비트 버전입니다. 이는 Windows에서 C, C++ 등의 프로그램을 컴파일하고 실행하는 데 사용됩니다. Git Bash는 이 MinGW64를 기반으로 하여 **Unix/Linux 스타일의 쉘 환경을 Windows에서 사용할 수 있게 해줍니다.**
- 노란색 : 현재 파일 위치
    - 파일위치에서 `~`는 사용자의 **홈 디렉토리**를 나타냅니다. 홈 디렉토리는 사용자가 기본적으로 작업하는 디렉토리이며, 각 사용자마다 고유한 경로를 가지고 있습니다. 예를 들어, `C:\\Users\\username`가 Windows에서의 홈 디렉토리 경로입니다. `~`는 이 홈 디렉토리를 나타내는 축약형으로 사용됩니다.
    - 리눅스는 항상 홈 디렉토리로 부터 시작한다.
    - cd ~ : 홈 디렉토리로 이동
    - cd - : 뒤로가기
    - cd .. : 상위 폴더
    - git init 명령어를 통해 시작가능
        - 숨겨진 파일을 지우면 종료된다.

## 명령어 모음

- touch : 파일 생성
- mkdir : 폴더 생성
- ls : 현재 경로에 있는 파일이나 디렉토리가 나타남
    - 명령어 `ls`는 "list segments"의 약자입니다. 이 명령어를 사용하면 현재 경로에 있는 파일과 디렉토리의 목록을 보여줍니다.
- cd : 경로 이동
    - ~ : 홈 디렉토리
    - - : 뒤로가기 ( 전에 있었던 디렉토리로 이동한다)
    - .. : 상위 폴더
- start : 파일 실행
    - bash의 가장 큰 장점
    - 윈도우 환경에서 왜 linux 기반 bash를 사용할까? 
    → **‘TAB’ 자동 완성 기능을 사용하기 위해서!**
- rm : 파일 삭제
    - 디렉토리를 삭제하려면 ‘-r’ 옵션을 넣어줘야한다

## vscode 단축키

- ctrl + ` , ctrl + j : 터미널 열기
- ctrl + w : 현재 파일 탭 닫기
- ctrl + tab : 탭 옮기기
- ctrl + shift + F : 전체 찾기
- alt 누른 상태에서 마우스 좌클릭 : 동시에 여러개의 커서 지정 가능
- shift + tab : 들여쓰기 취소
- ctrl + a : 전체 블록 지정
- ctrl + / : 주석 설정
- shift + insert : 터미널에 붙여넣기
- init

나머지는 수업 진행하면서 배우기!

## Git 사용법

- git : 분산 버전 관리 시스템
    - 각 버전은 이전 버전으로부터의 변경사항을 기록하고 있음
    - 중앙 집중식 VS 분산식
- Upload = Push
- Download = Pull
- 환경 복사 = Clone
- git clone (주소)
    - git config —global [user.email](http://user.email) “이메일”
    - git config —global [user.name](http://user.name) “닉네임”
- 전에 했던 history가 남아있어 덮어쓰기를 해도 사용가능하다.
- 자격 증명 관리 탭에서 git 관련 로그인 이력을 삭제 가능하다.]

### Git 실습

- 시작 : git init
- branch = master
- commit 작성자 변경하는 방법 (한번만 하면 OK)
    - git config —global user.name
    - git config —global user.email
    - git config —global -l (확인법)
- git 시작 확인하는 방법
    - 숨김 폴더 .git 생성
    - git bash에 (master) 표시가 생성됨
- add
    - git add .
        - . 은 현재 디렉토리를 의미함.
        - 특정 파일만 하려면 어떻게 해야될까?
            - git add d.txt ← 이런 방식으로 진행하면 OK!
            - **add → commit → push**
    - git status : 현재 진행 상태를 볼 수 있다.
        - 바로 commit 되는게 아닌, staged 상태로 들어가는 것이다.
- commit
    - git commit -m “0111 git test"
        - -m 은 메세지를 의미한다. commit 할 것들의 의미를 적어주면 좋다.
    - git log
        - commit이 잘 됐는지 확인할 수 있다.
- push
    - upload와 동일한 기능이다.
        - git remote add origin 주소
        - git remote -v
        - git push -u origin master : 처음 push  할 때 사용
        - git push origin + master : 강제로 덮어쓰기 하더라도 push 하겠다는 의미!
    - **clone 기능을 사용하면 remote를 할 필요가 없다.**

- QnA
    - master가 뭘까?
        - branch master로 설정되어있다 : git의 기본 branch는 항상 master로 설정되어있다.
    - branch는 뭔가요?
        - 코드를 개발하거나 수정하는 데에 사용되는 ‘작업 공간’
    - HEAD → master
        - HEAD : 현재 작업중인 commit
        - master : HEAD가 가리키는 branch 명
    - github ↔ gitlab
        - github 사용 용도
            1. 개인 프로젝트 작업 공간 (공부한 것 저장)
            2. 포트폴리오
            3. 프로젝트 협업

- **오늘 배운 내용 총정리**

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/11c46b42-5382-4dc7-961e-be37754766c7/ac5840d7-700f-4e88-af0e-a5b8f73a696f/Untitled.png)

- add 후 잘됐는지 확인 : git status
- commit 후 잘 됐는지 확인 : git log

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/11c46b42-5382-4dc7-961e-be37754766c7/5a62c3a1-41bd-4b7b-b9c1-da5e8e97130e/Untitled.png)

- git 은 로컬 저장소 내 모든 파일의 ‘변경사항’을 감시하고 있다.

- 원격 저장소
    - GitLab, GitHub, Bitbucket 등 존재
    - 사용법
    
    ```bash
    git remote add origin remote url
    ```
    
    1. git init → add, commit → remote → push (정배)
    2. git init → clone → add, commit, push (remote 할 필요 없음)
    
    ```bash
    git push -u origin master
    ```
    
    - 원격 저장소에 commit 목록을 업로드
        - 최초 push 시에는 github 로그인 필요
        - push는 clone, pull 과는 다르게 개인적으로 사용해야하기 때문이다
        - 원격 저장소에는 commit이 올라가는것
            - git log (HEAD → master) 잘됐는지 확인해보라.
        - 파일 수정 시 add 부터 다시 진행해야 한다
    
    ```bash
    git pull origin master
    ```
    
    - pull 과 clone 의 차이점이 뭘까?
        - 처음 프로젝트를 진행할 때는 ‘clone’
        - 작업 중 다른 인원이 변경한 사항을 업데이트할 때 ‘pull’
        - 'git pull'은 원격 저장소의 최신 변경사항을 로컬 저장소로 가져오는 명령어이고, 'git clone'은 원격 저장소의 모든 데이터를 복제하여 새로운 로컬 저장소를 생성하는 명령어입니다. 따라서, 'git pull'은 이미 로컬에 저장소가 있는 상태에서 원격 저장소의 변경사항을 업데이트할 때 사용하며, 'git clone'은 원격 저장소를 처음으로 로컬에 가져올 때 사용합니다.
    
    ## 오후반 - .getignore
    
    - **프로젝트에 따라 공유하지 않아야 하는 것도 존재하기 때문에 사용한다**
    - 이미 git의 관리를 받은 파일이나 디렉토리는 나중에 gitignore에 작성해도 적용되지 않음
    - 작성된 파일명은 push를 해도 전송되지 않는다.
    - gitignore 설정 서비스
        
        [gitignore.io](https://www.toptal.com/developers/gitignore/)
        
    - .gitignore은 텍스트 문서다.
        - 작성법
        1. 직접 입력하기
        2. echo c.txt >> gitignore
    
    - TIL : Today I Learned
        -