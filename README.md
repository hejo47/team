# 깃 명령어

```
echo "# team" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/hejo47/team.git
git push -u origin main
```

# 브랜치 전략

팀원
```
* 주의사항 : 비주얼 스튜디오 코드에서 작업할 때 작업폴더를 항상 루트폴더로 열기 *

처음 작업할 때
1. git clone 원격저장소 주소
2. git switch -c 사용할 브랜치 이름
3. 작업
4. git pull origin 풀 할 브랜치이름
5. git add .
6. git commit -m ""
7. git switch 풀 했던 브랜치 이름
8. git merge 자신의 브랜치 이름
5. git add .
6. git commit -m ""
9. git push origin 풀 했던 브랜치 이름

다시 푸쉬할 때
1. git switch 내 브랜치 이름
2. 작업
3. git pull origin 풀 할 브랜치이름
5. git add .
6. git commit -m ""
7. git switch 풀 했던 브랜치 이름
8. git merge 자신의 브랜치 이름
9. git pull origin 풀 할 브랜치이름
10. git add .
11. git commit -m ""
12. git push origin 풀 했던 브랜치 이름

```
# 배포하기(HEAD 이동, develop(a: 현재 작업 중) -> main(b))

팀장
```
git pull origin develop
git merge main
git add .
git commit -m "배포"
git push origin main

```

https://team-mocha-theta.vercel.app/