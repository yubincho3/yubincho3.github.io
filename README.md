# 빌드 과정

1. Ruby 다운로드  
다음 링크에서 WITH DEVKIT 최신 버전 다운로드  
**https://rubyinstaller.org/downloads/**  
2. jekyll 다운로드  
cmd 혹은 powershell에서 다음 명령어 입력:
**gem install jekyll bundler**  
3. 테마 적용  
다음 링크에서 minimal-mistakes 테마 다운로드  
**https://github.com/mmistakes/minimal-mistakes**  
4. GitHub repository 생성  
(NICKNAME).github.com으로 레포지토리 생성  
5. Repository clone  
다음 명령어를 입력해서 레포지토리 클론  
**git clone https://github.com/(NICKNAME)/(NICKNAME).github.com**  
6. 블로그에 테마 적용  
다운로드 받은 테마 폴더를 압축 해제하고 내용물을 레포지토리 로컬 저장소 폴더에 복사+붙여넣기  
7. 템플릿 채우기  
**_config.yml**의 프로필 이미지, 블로그 제목 등 비어있거나 기본 텍스트로 되어 있는 정보들을 자신의 정보로 수정  
8. 파비콘 적용하기  
다음 링크에서 파비콘으로 적용하길 원하는 이모지 입력 후 변환 후 다운로드 후 
**https://favicon.io/favicon-generator/**  
다운로드 받은 압축 파일 해제 후 내용물을 
로컬 저장소 폴더에 전부 붙여넣기  
9. Google Analytics 추가  
Google Analytics 생성 후 **_config.yml**의 **analytics** 속성의 **provider**를 **google-gtag**로, **tracking_id**에는 자신의 트래킹 ID를, **anonymize_ip**는 자유롭게 채운다.
10. 기타 커스텀  
폰트, 카테고리 등 원하는 요소들을 css 파일 및 html 파일 등을 수정하여 커스텀  
11. 최종 테스트  
**bundle exec jekyll serve --trace** 명령어로 최종 테스트를 하며 작동하지 않는 부분이 있다면 수정한다.  
12. 스테이징 및 커밋 반영  
다음 명령어를 순서대로 입력해서 파일 스테이징, 커밋, 푸쉬를 진행한다.  
**git add .**  
**git commit -m "MY COMMIT MESSAGE"**  
**git push**  
13. 블로그 확인  
블로그에 접속해서 정상적으로 반영되었는지 확인한다.  