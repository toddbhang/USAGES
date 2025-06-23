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

- 버전관리 필요없는 파일을 서버에서 삭제하고 로컬에 그대로 두기
  * .gitignore 팔일 설정하기
  * git rm --cached <파일경로>  (Git에서 캐시 제거)
  * git commit -m "Remove unnessary files from version contol"
  * git push origin <branch name> 

- 특정 폴더만 복원 (baremetal 폴더 만 복원) 
  * git checkout origin/main_r3 -- baremetal/
    
## Markup 사용법

### 1. 제목
```
# 제목 1
## 제목 2
### 제목 3
```

### 2. 굵게/기울임
```
**굵게**
*기울임*
```

### 3. 목록(List) 
```
- 순서 없는 목록
- 항목 2

1. 순서 있는 목록
2. 항목 2
```

### 4. 코드(Code) 
```
`인라인 코드`

'```
여러 줄 코드 블록
'```
```

### 5. 링크/이미지
```
[링크 텍스트](https://example.com)

![이미지 설명](https://example.com/image.png)
```

### 6. 인용문
```
> 인용문
```

### 7. 구분선
```
---
```

### 8. 표
```
| 헤더1 | 헤더2 |
|-------|-------|
| 값1   | 값2   |
```

