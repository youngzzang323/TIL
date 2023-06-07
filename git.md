### git : 분산 버전관리 시스템

작업을 하고
변경된 파일을 모아 (add)
버전으로 남긴다. (commit)

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

![커밋돌아가는 방법](/git%EC%9D%B4%20%EB%8F%8C%EC%95%84%EA%B0%80%EB%8A%94%20%EA%B7%B8%EB%A6%BC.PNG)

 - git log -1 : -1 최근 한줄만 보기
 - git log -1--oneline : 최근한줄 한줄로 보기

