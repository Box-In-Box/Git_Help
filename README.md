# Git_Help
### [깃 생성]
```
git init                                                //git 파일 생성
git config --global user.name "name"                 //아이디입력
git config --global user.email "email"      //이메일 입력
git config user.name 					//네임확인
git config user.email 					//이메일확인
git config --global alias.name NAME			//NAME을 name으로 명령어추가 
```
### [깃 기본조작]
```
:q 							//나가기
:wq 							//저장하고 나가기
git status 						//현재상태
git add -A  						//모든파일 추가
git commit -m "name" 					//name으로 커밋
git commit --amend					//최근 커밋한 내용 수정(덧씌우기)
```
### [삭제]
```
git rm --cached -A					//모든파일 add 이전
git reset "앞6자리" --hard 				//과거로 돌아가고 미래파일 삭제
git revert "앞6자리" 					//전 캡슐과 반대 캡슐로 생성
git reset --hard HEAD^ 					//이전 커밋으로 되림
```

### [브랜치]
```
git branch name						//name의 브랜치 생성
git branch 						//현재 브랜치 확인
git branch -a 						//로컬 + 깃허브 브런치 모두 보기
git checkout name 					//name 브랜치로 이동
git checkout -b name 					//name 브랜치를 만들고 name으로 이동
git checkout -b name1 origin/name2 			//origin의 name2브랜치를 로컬name1로 만듦
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
.gitignore 						//파폴 생성 후 안에 넣으면 github에 안올라감
git push origin master 					//깃허브에 maser를 orgin에 올림
git remote 						//원격 레파지토리
git pull						//깃허브 정보를 가져옴
git push						//커밋한 내용을 깃허브에 올림
git clone address 					//address 주소에 있는 파일을 가져옴
git fetch						//깃허브의 패치정보를 가져옴
git pull origin master 					//깃허브의 origin에서 지금 파일master를 변경
git push origin branchname 				//branchname을 올림
git push -f origin main 				//이전 커밋된 내용을 깃허브에 다시 올림
```

### [푸쉬 제목 변경]
```
git commit --amend -m "title" //마지막 저장한 커밋 title로 다시 저장
git push --force 커밋 덮어 씌우기
```
