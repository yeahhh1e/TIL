**API(Application Programming Interface)** : 두 소프트웨어가 서로 통신할 수 있게 하는 메커니즘

**Interface** : 사용자가 기기를 수비게 동작 시키는 데 도움을 주는 시스템

**UI(User Interface)** : 사용자와 소프트웨어 간의 상호 작용 시스템

seed

temperature 

top_p : 얻고자 하는 답변이나 내용에 따라 적절하게 부여해야 올바른 응답값

**CLI**

→ why ? 효율성, 정밀한 제어, 표준성

---

**GIT** : 분산 버전 관리 시스템

-git의 역할: 코드의 버전(히스토리)를 관리, 개발되어 온 과정 파악, 이전 버전과의 변경 사항 비교

-git의 3가지 영역

**Working Directory**: 실제 작업 중인 파일들이 위치하는 영역 (어떤 특정한 폴더를 git으로 관리하겠다) 내 로컬 컴퓨터에 있는 것

**Staging Area**: Working Directory에서 변경된 파일 중, 다음 버전에 포함 시킬 파일들을 선택적으로 추가하거나 제외할 수 있는 중간 준비 영역

**Repository**: 버전 이력과 파일들이 영구적으로 저장되는 영역. 모든 버전과 변경 이력이 기록됨

**Commit**: 버전. 변경된 파일들을 저장하는 행위이며, 마치 사진을 찍듯이 기록한다 하여 ‘snapshot’이라고도 함 

git init: 로컬 저장소 설정(초기화). git의 버전 관리를 시작할 디렉토리에서 진행

git add: 변경사항이 있는 파일들을 staging area에 올리는 것

git commit: staging area에 있는 파일들을 저장소에 기록 → 해당 시점의 버전을 생성하고 변경 이력을 남기는 것

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/cdc19b73-f5d5-40d0-b5ed-89a13f190283/25a9ef3b-e85f-4d43-b7dc-5503d9ce4831/Untitled.png)

**git init**: 로컬 저장소 설정(초기화) git의 버전 관리를 시작할 디렉토리에서 진행

**git add**: 변경사항이 있는 파일을 stagig area에 추가

**git commit**: staging area에 있는 파일들을 저장소에 기록 → 해당 시점의 버전을 생성하고 변경 이력을 남기는 것

**git log —oneline** : commit 목록 한 줄로 보기

**git config --global -l**: git global 설정 정보 보기

*git 로컬 저장소 내에 또다른 git 로컬 저장소를 만들지 말 것

- 즉 이미 git 로컬 저장소인 디렉토리 내부 하단에서 git init 명령어를 다시 입력하지 말 것
- git 저장소 안에 git 저장소가 있을 경우 가장 바깥 쪽의 git 저장소가 안쪽의 git 저장소의 변경사항을 추적할 수 없기 때문
- .git 파일이 있는 곳이 working directory

vim : git commit 할 때 메세지 안 남기면 뜨는 창

vi a.txt → vim 으로 수정 가능

cat a.txt → 보기

i 누르면 insert라고 뜨면서 수정이 가능함

수정 후 esc 눌러 insert 나온 후 shift+ : 누르면 명령어 모드가 됨 q(그냥 종료)혹은 :wq (저장 후 종료)

TIL 폴더(Today I Learned)

-바로 직전 생성한 commit 수정하기

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/cdc19b73-f5d5-40d0-b5ed-89a13f190283/ac15341a-44a8-48a7-93f2-890cf90beda3/Untitled.png)

이게 바로 직전 수정한 commit

hash 값 확인 = 8f9463c

git commit —amend

원격 저장소: 코드와 버전 관리 이력을 온라인 상의 특정 위치에 저장하여 여러 개발자가 협업하고 코드를 공유할 수 있는 저장 공간

| git remote add origin remote_repo_url | 로컬 저장소에 원격 저장소 추가 |
| --- | --- |
| git remote add origin remote_repo_url | 별칭을 사용해 로컬 저장소 한 개에 여러 원격 저장소를 추가 할 수 있음 (origin : 추가하는 원격 저장소 별칭) |
| git push origin master | 원격 저장소에 commit 목록을 업로드 |
| git pull origin master | 원격 저장소의 변경사항만을 받아옴 (업데이트) |
| git clone remote_repo_url | 원격 저장소 전체를 복제 (다운로드)
→ clone으로 받은 프로젝트는 이미 git init이 되어 있음 |

-clone: local repo가 없을 때 다운 받는 것

-pull: 동기화(업데이트)

gitignore

.gitignore 파일 생성