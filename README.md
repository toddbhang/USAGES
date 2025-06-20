# USAGES 

## GIT 사용법 

- 로컬 폴더에서 Git 초기화
  * 내 프로젝트로 이동
  * git init
  * git add
  * git commit -m "first commit"
    
- github 저장소 연결
  * git remote add origin https://github.com/~~~
  * git branch -M main
  * git push -u origin main
    
- github 프로젝트 내려받기
  * git clone http://github.com/~~
 
- git 수정사항 확인
  * git status (변경파일, 추적되지 않는 파일) 
  * git diff (상세 변경 내용 확인)0 
  * git diff --staged (git add로 스태이징된 변경내용)
  * git log (최근 커밋 로그 보기)
  * git diff 파일 이름
 
- github commit
  * git add .
  * git commit -m "메시지"
  * git push origin main
  * git add 파일이름
  * git ocmmit -m "메시지"
  * git push origin main
 
- 실수했을때
  * git commit --amend
 
- 실수한 커밋되돌리기
  * git commit --amend (방금한 커밋 메시지만 고치기)
  * git reset --soft HEAD~1  (커밋취소, add 그대로, 수정된 내용 그대로)
  * git reset --mixed HEAD~1 (커밋,add 취소, 수정된 내용 그대로)
  * git reset --hard HEAD~1 (커밋, add, 수정된 내용 모두 완전취소)
  * git reset 커밋해쉬 (이미 푸쉬한 커밋을 되돌림)
  * git log --oneline (커밋 내역) 
- 
