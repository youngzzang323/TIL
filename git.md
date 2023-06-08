### git : 분산 버전관리 시스템

작업을 하고
변경된 파일을 모아 (add)
버전으로 남긴다. (commit)
 ## git 기본

터미널에서 git bash를 눌러서시작한다
1. git init - git을 사용한다(저장소 초기화)
 - touch : 파일만들기
 - git status : git 상태
 - git add . -모든파일 깃에등록?
 - git commit -m '메시지' : 커밋

 - git log : 커밋 기록보기

2. - git init: git 디렉토리 생성
- git status: 현재 git 디렉토리의 상태를 보여줌.
- git add .(또는 파일): 현재 변경된 파일들을 모으는 작업.
- git commit =m ‘메시지’: git add로 모아진 파일들의 버전을 남기는 명령어. 메시지는 커밋에 대한 설명을 작성한다.
- git log: commit한 기록을 보여줌
- cd 폴더이름 : (change directory)  : 폴더 바꾸기
![커밋돌아가는 방법](/git%EC%9D%B4%20%EB%8F%8C%EC%95%84%EA%B0%80%EB%8A%94%20%EA%B7%B8%EB%A6%BC.PNG)

 - git log -1 : -1 최근 한줄만 보기
 - git log -1--oneline : 최근한줄 한줄로 보기


## 원격 저장소

3. github 원격저장소
 - git remote add  origin https://github.com/youngzzang323/TIL.git : 깃 origin 이라는 이름으로 주소저장
 - git remote -v 원격저장소 이름 url정보확인
 - git push origin(원격저장소이름) main(브랜치이름)
 - git remote rm origins : 원격저장소 내용 삭제

## git오류메세지

4. 오류 메세지
 - Untracked : 한번도 커밋 된 적 없는 파일(디렉토리에만있음)
 - changes not staged for commit : 스테이지에 파일없음
 - nothing to commit, working tree clean : add를 한 파일 자체가없다,이전 커밋대비 변경사항없음

## 공유하지 않는 git 파일 설정
 5. 공유하면 안되는 파일(github에 올리지 않을 파일 설정)
 -  .gitignor파일을 만들어서 안에 버전파일들을 안에넣고 .gitignor add해주면됌
 - *.csv : 마지막이 csv로 끝나는 모드파일

## 협업 등을 위한 branch merge
 6. 협업!(merge) - 각 branch에서 작업하고 merge로 합친다.

  - 같은 파일이 수정되면 충돌이 발생한다.
  - pull : fetch + merge의 합쳐진 기능을한다고 생각하면 된다.
  - git branch <브랜치이름> : 브랜치생성
 - git checkout <브랜치이름> : 브랜치이동
 - git checkout -b <브랜치이름> : 브랜치 생성및이동
  - git branch : 브랜치 목록
  - git branch -d <브랜치이름> : 브랜치 삭제

## pull request 하기 (main에서 하면 안됌)
  7. 다른사람 github에서 Fork 하기
    - main 프로젝트의 주소에 들어가서 'Fork' 클릭하고 Create Fork 클릭
원격저장소에 clone해야함. (반드시 나의 저장소에 클론해주어야 한다.)
- git clone https://github.com/(%EB%82%98%EC%9D%98 원격저장소 주소)/(fork한 name)
- 명령어는 바탕화면에서 git bash 또는 terminal을 열어서 입력해준다.
- git 저장소가 아닌 곳에서 (main표기가 없는) 입력해주면 된다.
- 바탕화면에 fork 받은 폴더가 있는데 이것을 vs code로 열어서 코드 작성 진행.
- 작성이 끝나면 add, commit, git push origin main 진행
- Github에 들어가서 Pull Request 만든다.
