```
Sazasaza homepage build
@author: sangmoklee
@date: 2022-Jun
```

## **Objectives**
* 카페 24 jsp 호스팅
* 서버는 tomcat 기반


## **Folder tree**  (default 경로 : /sazasaza12/tomcat/webapps/ROOT/)
```
**<참고 사이트> **
https://velog.io/@woo0_hooo/%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8-%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%B9%B4%ED%8E%9824%EC%97%90%EC%84%9C-%ED%98%B8%EC%8A%A4%ED%8C%85%ED%95%98%EA%B8%B0 (카페 24호스팅 관련_1)
https://shelley-in-2020.tistory.com/5 (카페 24호스팅 관련_2)

https://gspkr.tistory.com/76 (jsp 디비 연결)

https://jin2rang.tistory.com/entry/%ED%86%B0%EC%BA%A3%EC%84%9C%EB%B2%84-%EC%84%A4%EC%A0%95-%EB%B0%8F-%EC%8B%A4%ED%96%89%ED%95%98%EA%B8%B0-A-to-Z (파일구조 설명)


---- folder
- file

cd /tomcat/webapps/ROOT/
    |
    |- index.html                   : 메인 화면
    |- login.html                   : 로그인 화면
    |- sing-product.html            : 제품 상세화면
    |
    |---- **css**                   
    |                               
    |- style.css                    : 메인 css
    |- responsive.css               : 서브 css
    |- login.css                    : 로그인 css
    |                                 
    |---- **image**                 : 관련 이미지 파일
    | 
    |---- **js**
    |
    |- script.js                    : 기본 js
    |- signup.js                    : 로그인 관련 js
    |
    |---- **WEB-INF**               
    |
    |- web.xml                      : 설정 xml파일이 있음. DB열어주는 설정 할 때 수정 필요
    |
    |- index.jsp                    : 카페 24 기본 배경화면
    |- index.jsp.default.             카페 24 기본 배경화면
    |
    |- mysql.jsp                    : 홈페이지 디비 연결용(test중...)
    |
```


* **홈페이지 접속방법**
    * 카페 24 호스팅 확인 (https://www.cafe24.com/)
         * ID: sazasaza12
         * 비:  saza1q2w3e~
         * FTP,SSH,DB 비밀번호 : saza1q2w3e!

* **ssh 접속 정보**
    * 윈도우는 putty로 접속하면 됨, Mac은 터미널에서 직접 접속 가능
        * ssh sazasaza12@sazasaza12.cafe24.com
        * 비밀번호 : saza1q2w3e!
   
    * DB - 서버는 홈페이지 로컬에 있음 (maria DB)
        * mysql -u sazasaza12 -p 
        * 비밀번호 : saza1q2w3e!

* **파일전송의 경우 filezila 사용하면 됨**

* **도커 환경구성 방법**
    * [https://shanepark.tistory.com/307](https://shanepark.tistory.com/307) - 도커 톰캣환경 설치
    * [https://shanepark.tistory.com/307](https://shanepark.tistory.com/307) - 도커 한국시간 설정
    * [https://sharplee7.tistory.com/75](https://sharplee7.tistory.com/75) - 도커 디비연결관련1
    * [https://yooloo.tistory.com/171](https://yooloo.tistory.com/171) - 도커 디비연결관련2
    * [https://gspkr.tistory.com/76](https://gspkr.tistory.com/76) - 도커 디비연결관련3


