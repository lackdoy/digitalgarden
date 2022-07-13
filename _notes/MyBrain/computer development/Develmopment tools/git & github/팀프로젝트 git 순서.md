### Date : 2022-06-15 16:02

### Topic : 팀프로젝트 git 순서
---
### Summary
> git을 이용한 프로젝트 진행의 순서를 알아보자. 

#### Order :
- github에 repository 생성
- Repository의 Link 복사
- Local PC의 project root folder 경로 이동
- git init 실행 (.git 숨김폴더 생성여부 확인)
- github와 연결하기 위하여 git remote add origin (link)/project_name 입력
- connecting 여부를 확인하기 위하여 git remote -v 명령어 실행
- Master(Main) branch를 내걸로 수정해주는 작업 진행해야함
- git branch feature/subMaster(mybranch)
- git checkout feacture/subMaster(myranch)
- git branch로 현재 branch 위치 확인
- 코딩작업 시작
- 코딩 완료 후, git add (작업한 파일의 이름) 명령어 입력
- 또는 git add --all 입력
- add한 작업을 스테이징에서 원격에 올리기 위해 commit 진행
- git commit -m "commit comment writing area"
- git push 를 통해 올리기
- git push (저장소이름) (branch name)
- 
### Reference
- 

### Link
-
