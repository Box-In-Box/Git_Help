# Git_Help
### [깃 생성]
```
git init                                                //git 파일 생성
git config --global user.name "dgf0000"                 //아이디입력
git config --global user email "dgf0000@naver.com"      //이메일 입력
git config user.name 					//네임확인
git config user.email 					//이메일확인
```
### [깃 기본조작]
```
:q 							//나가기
:wq 							//저장하고 나가기
.gitignore 						//파일 생성하면 github에 못올림
git status 						//상태
git add -A  						//모든파일 넣기
git add .  						//모든파일 넣기
git commit -m "name" 					//name 의 제목
```
### [삭제]
```
git reset "앞6자리" --hard 				//과거로 돌아가고 미래파일 삭제
git revert "앞6자리" 					//전 캡슐과 반대 캡슐로 생성
```

### [브랜치]
```
git branch name						// name의 브랜치 생성
git branch 						//현재 분기점 확인
git branch -a 						//로컬 + github 브런치 모두 보기
git checkout name 					// name 브랜치로 이동
git checkout -b name 					//name브랜치 만들고 name 으로 이동
git checkout -b name1 origin/name2 			//origin의 name2브랜치를 로컬name1로 만듬
git branch -D name 					//name 브랜치 삭제
```

### [로그]
```
git log	                                                //로그확인
git log --graph --all --decorate 			//UI 로그
```

### [브랜치 통합]
```
git merge name 						//name의 브랜치 값을 가져옴(병합)
git rebase name 					//name의 브랜치 값을 가져옴(재배치)
```

### [깃허브 조작]
```
git push origin master 					//github에 maser를 orgin에 push
git remote 						//원격 레파지토리
git push						//commit 한 내용을 git에 push
git clone address 					//address 주소에 있는 파일을 가져옴
git fetch						//github의 패치정보를 가져옴
git pull origin master 					//github의 origin에서 지금 파일master를 변경
git push origin branchname 				//branchname을 push
```
