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
git pull origin 풀 할 브랜치이름
git switch -c 이름 // 자신 이름 브랜치 생성
자신의 이름으로 된 파일을 만든다.

git commit -m ""
git switch 풀 했던 브랜치 이름
git merge 스위치 했던 브랜치 이름
git add .
git commit -m ""
git push origin 풀 했던 브랜치 이름

```