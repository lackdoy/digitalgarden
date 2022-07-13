### Date : 2022-06-15 16:02

### Topic : git을 사용하는 용어와 명령어
---
### Summary
> git의 기능을 쓰기 위해서는 명령어(command)들과 그 명령어들을 사용하는 순서에 대해서 이해하고 있어야 한다. 각각의 명령어들과 명령어들에 포함되는 단어에 대해서 이해해야만 프로젝트를 운용하는데 큰 문제가 없을 것이다.

#### Basic word:
- Local  : 개인 PC or 노트북
- Remote : 원격의 환경(Git server nas)
- Repository : 깃에서 팀원들고 프로젝트를 저장, 공유할 수 있는 원격 저장소(공유폴더)
- clone : 원격지에 저장되어있는 모든 데이터를 Local로 복사해옴
- Fork : 등록된 Repostiory가 아닌 다른 Repository를 본인의 Repostiory로 복제해옴
- Commit : 형상관리를 위한 기록 수단 (코드에 누가 언제 무엇을 어떻게 했는지 기록함)
- Push : Local repository의 데이터를 Remote Repostiory로 업로드함
- Pull : Remote Repostiory의 데이터를 Local Repostiory로 내려받음
- Working directory : 개발자의 현재 시점으로 소스코드를 수정하며 개발하는 공간
- Staging Area : working directory에서 작업한 파일을 Local Repository로 전덜하기 위해 파일을 분류하는 공간
- Branch : Remote Repository의 현재 상태를 복사하여 master branch와 별개의 작업을 진핼할 수 있는 공간(보통 Branch를 생성하고 개발한 다음 개발이 완료되면 master branch에 merge 하는 방법으로 소스코드를 합침)
- Head : 현재 작업중인 브랜치의 최근 commit된 location
- Index : Staging Area를 의미
- Pull Request(PR) : Push된 Commit 사항을 깃헙에 공유하는 작업
- Merge : PR에 대한 관리자 승인이 났을 경우 merge가 일어남.

#### Command list:
- git add : 수정된 소스코드를 Staging Area에 전달
- git commit : add된 모든 소스코드를 Local Repository에 전달
- git push : Local Repository에 적용된 모든 변경사항을 Remote Repository에 전달
- git pull : Remote Repository에서 변경된 파일들을 모두 Local Repository에 전달
- git fetch : Remote Repository에서 변경된 파일들을 모두 Local Repository에 전달 (단, fetch를 하더라도 IDE 등의 작업공간에는 변경사항이 적용되지 않음)
- git merge : LocalRepository에서 변경이 발생한 파일들을 workingDirectory로 전달 (IDE 등의 작업공간에 변경사항 적용됨)
- git init : RemoteRepsitory와 연동하기 위하여 빈 git 저장소 만들기
- git branch : 생성되어있는 브랜치를 확인
- git branch {name} : name이라는 이름으로 새로운 branch 생성
- git checkout {name} : 현재 브랜치를 name이라는 이름으로 변경
- git status : WorkingDirectory에서 수정이 발생된 파일들을 확인
- git clone : Remote Repository에 저장되어있는 모든 파일을 Local Repository에 복사
- git reset {soft/mixed/hard} : 작업된 파일들을 특정 커밋 위치로 리셋.
- git log 작업내역 시각화 확인하기

### Reference
- https://velog.io/@amdye2323/%ED%8C%80%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-GIT-%EB%AA%85%EB%A0%B9%EC%96%B4-%EC%88%9C%EC%84%9C [amdye2323.log] 팀프로젝트 GIT 명령어 순서

### Link
-[[How to start github]]
