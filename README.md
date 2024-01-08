# Team Project 연습

## git repository 생성하기 : 팀장이 팀프로젝트 생성
* 원격 Repository 생성하기

* 로컬 Repository 생성 및 동기화
```bash
mkdir TeamProject
cd TeamProject

git init
git remote add origin...
git commit -m "커멘트"
git push -u origin master
```

## Collaborators
* 원격 Repository 의 `Settings/Collaborators` 메뉴에서 (git)회원 id 검색하여 추가하기
* 추가된 회원은 본인 email 에서 확인하기

## 원격 Repository clone 하기
* 각 회원들은 팀장의 원격 Repository 를 `workspace` 폴더에서 `clone` 하기
* clone 한 프로젝트 폴더에서 다음 작업 계속하기 

## 주의사항
* 절대 같은 파일을 두 명 이상이 편집하지 않는다.
* `.gitignore` 파일 관리를 잘 해야 한다. 만약 ide 도구등에서 자동으로 변경되는 파일들이 repository 에 섞여서 push 될 경우 여러가지 문제를 일으킨다.
* 반드시 `branch` 를 구분해야 한다.

## branch 분리하기 : 매우 중요!!!
* `git checkout -b branch명` 밑의 두 개의 명령어를 합친것 이렇게 많이 사용
* `git branch branch명`, `git checkout branch명`
* checkout 를 실행하면 새로운 branch 작업환경이 전환된다.

* 프로젝트 진행하기...

## 작업한 내용 원격 repository 에 commit(push) 하기
* `git add .`
* `git commit -m "커멘트`
* `git push origin yangtory` :  작업하고 있는 branch명 반드시 써주기