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
<<<<<<< HEAD
<<<<<<< HEAD
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
=======
<<<<<<< HEAD
git pull origin 풀 할 브랜치이름
git switch -c 이름 // 자신 이름 브랜치 생성
자신의 이름으로 된 파일을 만든다.

git commit -m ""
git switch 풀 했던 브랜치 이름
git merge 스위치 했던 브랜치 이름
git add .
git commit -m ""
git push origin 풀 했던 브랜치 이름
>>>>>>> 28476b2f256304b6c0c902a54972a34e1899d5da

```
=======
=======
>>>>>>> 6cc1877758c7b4bdff462a3631bdfa19af999351
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

```

# 배포하기(HEAD 이동, develop(a: 현재 작업 중) -> main(b))

팀장
```
git checkout develop
git reset —hard main
git push -f origin main
```

