---
title:  "[Blog] jekyll 블로그에 Google Analytics 추가하기(minimal-mistakes)" 

categories:
  - Git
tags:
  - [Blog, Google, minimal-mistakes]
---

## Google Analytics란?  
![화면 캡처 2022-11-28 164259](https://user-images.githubusercontent.com/64318704/204221165-c992406f-6c31-4cb2-9a92-2daa2a7a8826.png)  
웹사이트의 트래픽을 추적하여 통계로 보고해주는 서비스다.   
통계 서비스를 이용하여 웹사이트의 방문자에 대한 자세한 정보를 알 수 있다.  
## 설치하는 방법  
![화면 캡처 2022-11-28 164658](https://user-images.githubusercontent.com/64318704/204221929-735d8c2a-26bd-4de8-b929-b8b64570a0c7.png)  
Google Analytics 사이트\([링크](https://analytics.google.com/)\)에 접속하여 측정 시작을 누른다.  
  
![1](https://user-images.githubusercontent.com/64318704/204222326-42846d02-9f9c-49fa-ba9b-6ed4711cf67e.png)  
![2](https://user-images.githubusercontent.com/64318704/204222586-8fba272b-c388-4b8b-9ef4-b506d3681199.png)  
계정 이름을 자유롭게 짓고, Google 제품 및 서비스 항목을 체크한다.\(더 자세한 통계를 얻을 수 있다.\)  
  
![1231](https://user-images.githubusercontent.com/64318704/204223080-95db4ca0-43b0-49f3-9249-a613213e7a17.png)  
속성 이름 또한 자유롭게 짓고 시간대와 통화를 맞춰주자.  
이후 비즈니스 정보를 자신의 목적에 맞게 작성하고 만들기를 누른다.\(약관은 전부 동의\)  
  
![platy](https://user-images.githubusercontent.com/64318704/204223601-1d46d80f-391e-4c14-8176-1a0af27b8506.png)  
![end](https://user-images.githubusercontent.com/64318704/204223805-973fc6be-ae5b-4524-b175-c4a45df2232b.png)  
이후 뜨는 화면에서 웹 플랫폼을 선택하고 자신의 웹사이트 정보를 작성하고 스트림을 생성해주자.  
  
![stream](https://user-images.githubusercontent.com/64318704/204224056-c6f22059-a9e7-4f45-8dcb-3b43a71aca9a.png)  
생성된 스트림의 측정 ID를 복사한다.\(URL과 이름은 임의로 입력했다.\)  
  
![config](https://user-images.githubusercontent.com/64318704/204224302-be3cc832-47c7-43fb-8be6-113651f2947d.png)  
그리고 **_config.yml**에 있는 analytics 항목의 provider를 **google-gtag**로,  
tracking_id에는 자신의 측정 ID를 입력해주자.  
그러면 변경된 항목들을 커밋 및 푸쉬해주면 끝.  
