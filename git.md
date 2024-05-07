# github

## git 초기 설정
> 사용자 이름, 이메일 주소 설정하기
```
git config --global user.name "본인이름"
git config --global user.email "본인 이메일 주소” 
```
__하는 이유__: 나중에 commit을 할때 사용자 이름과 이메일이 기록되기 때문이다.

제대로 했는지 확인하기 위해
```
git config --list
```
를 써본다

## github 초기 업로드
초기 업로드를 하기 전에  repository를 생성해야 한다

이후 vscode 터널을 연다
> 터미널 단축키
>
>- __cmd + j__ : 터미널 열기/닫기
>- __ctrl + c__ : 현재 실행중인 명령어 중지

__저장소 만들기__
```
git init 
```
__추가할 파일 더하기__
```
git add .
```
__히스토리 만들기__
```
git commit -m “메세지”
```
__레파지토리랑 vscode연결__
```
git remote add origin til링크
```
__깃허브에 업로드__
```
git push origin main
```

### 컴잇하기
```
git add .
git commit - m "내 메시지"
git push origin 브렌치명
```

## 만약 다른곳에 컴잇했다면

```

git reset HEAD^

git push origin main -f

git remote rm origin

```
__하고 없에고__

__다른곳에 올릴때__

```
git remote add origin til링크
git add .
git commit - m "내 메시지"
git push origin 브렌치명
```