# Tue11 스터디 190326

> 멋쟁이 사자처럼 화요일 오전 11시 스터디의 소개페이지입니다.
> 
> [홈페이지 링크](https://injoon35.github.io/study_introduce/)


## 오늘 한 것
1. 과제 검사
2. 과제 합치기
3. Git 명령어
4. 부트스트랩 그리드

## 1. Git
> CLI! 커맨드라인을 정확히 입력하자


1. 프로젝트 폴더에 깃폴더를 생성하는 명령어 (한번만)
``` shell
git init
```


2. **변경 내용을 추가하고 커밋 메시지 생성 (수시로 함)**
``` shell
git add .
git commit -m "커밋 메시지!"
```


3. Origin이라는 이름의 Remote를 추가함 (한번만)
> clone으로 받아왔다면 안해도 됨!
``` shell
git remote add origin GIT주소
```


4. **origin으로 커밋을 보냄 (수시로 함)**
``` shell
git push origin master
```


5. **서버에서 변경 내용을 가져옴 (수시로 함)**
> 만약 충돌이 났다면 충돌난 파일에서 변경사항을 조정해주시고
> 
> 2번 4번을 다시해주세요! (커밋을 다시 만들어주세요)
``` shell
git pull origin master
```


1. Git 레포지토리를 복제해옴 (한번만)
``` shell
git clone GIT주소
```


## 2. Bootstrap Grid
> 그리드 시스템에 대해 알아보았습니다.
> 
> 먼저 row를 설정하고 그 안에 12개의 열이 있다고 생각해주세요.
> 
> 예를 들면 6이라고 한다면 6/12 이므로 화면의 절반을 차지할 것입니다.
> 
> 아래의 코드를 통해 확인해주세요!


``` html
<div class="row">
    <!-- 스마트폰 때는 3등분 태블릿은 4등분 PC는 2등분 -->
        <div class="col-4 col-md-3 col-lg-6">
                <a href="/study_introduce/sanghee/index.html">박상희의 소개페이지입니다.</a>
            </div>
        <div class="col-4 col-md-3 col-lg-6">
            <a href="/study_introduce/injoon/index.html">최인준의 소개페이지입니다.</a>
        </div>
</div>
```

더 알고 싶다면 

[부트스트랩 레퍼런스 링크](https://getbootstrap.com/docs/4.3/layout/grid/)
