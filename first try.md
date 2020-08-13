# HTML
* 컨텐츠의 구조를 정의하는 마크업 언어

>> <마크> 컨텐츠 <마크>

## 첫번째 실습
~~~
<!doctype html>
<html>
    <head>
     <meta charset="utf-8">
     <title>like lion 8th</title>
    </head>
    <body>
     <h1>첫 실습</h1>
     <p>첫 실습이라구~~~</p>
    </body>
</html>
~~~~

### 코드 설명

* <!DOCTYPE html>
>> html 문서에 제일 처음에 와야하고 문서 형식을 정의함. 브라우저에게 문서 형식을 알려주는 역할

* <html lang="kr">
>> html에서 딱 한번만 쓰임. 
>> lang = language
>> 본격적인 태그의 시작, 사용하는 주 언어를 정의
  
* <head>
>> html의 문서에 대한 정보를 담고 있음.
>> 문서에서 단 하나 존재하며 html 아래에 위치

* <met acharset="utf-8>
>> html에서 쓰이는 한글이 깨지지 않도록 함
  
* <title>
>> 브라우저의 제목으로 쓰임
  
* <body>
>> 실질적으로 보여지는 부분
>> html 태그 안에서 한 번만 쓰임
  
## 레이아웃 태그

* header
>> 웹페이지 혹은 섹션의 제목을 담기위한 태그

* nav
>> 내비게이션 역할을 하는 요소, 페이지 이동을 하기 위한 메뉴를 주로 담음

* section
>> 기준에 따라서 구획을 구분하기 위해 사용되는 요소

* article
>> 주 내용을 담기 위한 태그

* aside
>> 광고나 사이트의 주변 부분에 해당하는 내용을 담기 위해 사용되는 태그

* footer
>> 웹사이트의 가장 아래에서 회사, 사이트 정보를 담기위해 사용되는 요소

~~~~
<!DOCTYPE html>
 <html>
 <meta charset='utf-8'>
  <head>
   <title>원돌일보</title>
  </head>
  <body>
   <header>
    <p>여기는 로고의 이름</p>
   </header>
   <nav>
    <p>여기는 사이트 이름</p>
   </nav>
   <section>
    <p>여기는 기사</p>
    <article>
     <p>첫번째 기사</p>
    </article>
    <article>
     <p>두번째 기사</p>
    </article>
   </section>
   <aside>
    <p>여기는 광고</p>
   </aside>
   <footer>
    <p>회사 정보</p>
   </footer>
  </body>
 </html>
~~~~~

## 순서
>> doctype - html - title - head - body - header - content - footer

