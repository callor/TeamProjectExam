# Team Project 연습

## git repository 생성하기 : 팀장이 팀프로젝트 생성
* 원격 Reposirogy 생성하기

* 로컬 Repository 생성 및 동기화
```bash
mkdir TeamProject
cd TeamProject

git init
git remote add orign ....
git commit -m "커멘트"
git push -u origin master
```

## Collaborators 설정하기
* 원격 Repository 의 `Settings/Collaborators` 메뉴에서 (git)회원 id 검색하여 추가하기
* 추가된 회원은 본인 email 에서 확인하기

## 원격 Repository clone 하기
* 각 회원들은 팀장의 원격 Repository 를 `workspace` 폴더에서 `clone` 하기
* clone 한 프로젝트 폴더에서 다음 작업 계속하기

## 주의사항 
* 절대 같은 파일을 두명 이상이 편집하지 않는다.
* `.gitignore` 파일 관리를 잘 해야 한다. 만약 ide 도구등에서 자동으로 변경되는 파일들이 repository 에 섞여서 push 될경우 여러가지 문제를 일으킨다.
* 반드시 `branch`를 구분해야 한다.

## branch 분리하기 : 매우 중요한 내용
* `git checkout -b branch명`
* `git branch branch 명`, `git checkout branch`
* checkout 를 실행하면 새로운 branch로 작업환경이 전환된다.

* 프로젝트 진행하기...

## 작업한 내용 원격 repository 에 commit(push) 하기
* `git add .`
* `git commit -m "커멘트" `
* `git push origin callor` : 작업하고 있는 branch 명 반드시 써주기

## pull request 하기
* 원격 repository 에서 자신이 올린 branch 를 선택
* `compare & pull request` 요청하기
* 이때 가급적이면 pull request 를 요청한 이유를 상세하게 작성하기
* `pull request` 버튼 클릭하여 요청완료

## 팀장이 `merge` 하기
* 프로젝트의 상단 메뉴에서 `pull request` 배지 확인
* 해당 pull request 를 열고 내용 확인하기
* 확인 완료되고 정상 pull request 임이 확인되면, `merge` 하기

## 팀원들이 merge 된 프로젝트 pull 하기
* 로컬 repository 에서 다시 master branch 로 이동 : `git checkout master`
* 원격에서 pull 해오기 : `git pull origin master`

## 팀원들이 자신의 작업 branch 와 master 동기화 하기
* 작업 brach 로 이동 : `git checkout callor`
* master 와 동기화 : `git merge master`