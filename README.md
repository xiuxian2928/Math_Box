# 수학 계산을 위한 코드를 제공하는 프로젝트
**1. calculator.py** : `계산기`에 있는 기능들을 제공하는 모듈
- add, subtract 등

### ** git 커맨드 정리 **
- git push -u origin master : 로컬 레포지토리의 내용을 처음으로 리모트 레포지토리에 올릴 때 사용합니다.(-u origin master가 무슨 뜻인지는 'Git에서 브랜치 사용하기' 챕터에서 배울 거니까 걱정마세요!)
- git push : 로컬 레포지토리의 내용을 리모트 레포지토리에 보내기 
- git pull : 리모트 레포지토리의 내용을 로컬 레포지토리로 가져오기
- git clone [프로젝트의 GitHub 상 주소] : GitHub에 있는 프로젝트를 내 컴퓨터로 가져오기

### ** git 커밋 다루기 **
- git log : 커밋 히스토리를 출력
- git log --pretty=oneline : --pretty 옵션을 사용하면 커밋 히스토리를 다양한 방식으로 출력할 수 있습니다. --pretty 옵션에 oneline이라는 값을 주면 커밋 하나당 한 줄씩 출력해줍니다. --pretty 옵션에 대해 더 자세히 알고싶으면 이 링크를 참고하세요. 
- git show [커밋 아이디] : 특정 커밋에서 어떤 변경사항이 있었는지 확인
- git commit --amend : 최신 커밋을 다시 수정해서 새로운 커밋으로 만듦
- git config alias.[별명] [커맨드] : 길이가 긴 커맨드에 별명을 붙여서 이후로 별명으로 해당 커맨드를 실행할 수 있도록 설정
- git diff [커밋 A의 아이디] [커밋 B의 아이디] : 두 커밋 간의 차이 비교
- git reset [옵션] [커밋 아이디] : 옵션에 따라 하는 작업이 달라짐(옵션을 생략하면 --mixed 옵션이 적용됨) 
-- (1) HEAD가 특정 커밋을 가리키도록 이동시킴(--soft는 여기까지 수행)

-- (2) staging area도 특정 커밋처럼 리셋(--mixed는 여기까지 수행)

-- (3) working directory도 특정 커밋처럼 리셋(--hard는 여기까지 수행)

-- 그리고 이때 커밋 아이디 대신 HEAD의 위치를 기준으로 한 표기법(예 : HEAD^, HEAD~3)을 사용해도 됨

- git tag [태그 이름] [커밋 아이디] : 특정 커밋에 태그를 붙임
