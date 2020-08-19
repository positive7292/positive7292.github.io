# 11강

## 텍스트와 관련된 속성

### 폰트

* font-size

>> 크기

* font-family

>> 폰트의 종류

>> 첫번째가 없으면 두번째가 설정이 되게 해야 함

>> 예시 'cute font', Arial, cursive

>> 웹 폰트 : 웹에서 링크를 통해 폰트를 불러오는 방식
~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <title>실습</title>
      <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">
    <style>
      #main {
           font-family: 'Roboto', sans-serif;
      }
    </style>
    </head>
    <body>
      <div id="main">
      <
    </body>
  </html>
</div>
~~~

* font-size
~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <title>실습</title>
      <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">
    <style>
      #main {
           font-family: 'Roboto', sans-serif;
           font-style: oblique;
      }
    </style>
    </head>
    <body>
      <div id="main">
      <
    </body>
  </html>
</div>
~~~
>> normal, italic, oblique가 있음

* font- weight


>> 폰트 굵기, bold or 100 ~ 900 중의 숫자를 사용할 수 있음
~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <title>실습</title>
      <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">
    <style>
      #main {
           font-family: 'Roboto', sans-serif;
           
      }
    </style>
    </head>
    <body>
      <div id="main">
      <
    </body>
  </html>
</div>
~~~

#### 폰트 속성 하나로 4가지 속성을 모두 적용 가능

>>> 예시 font : oblique 900 35px 'Roboto', sans-serif;

## 텍스트 정렬과 관련된 기능

* text-align

>> 텍스트를 좌, 우, 중앙 정렬을 할 때 씀
~~~
>> normal, italic, oblique가 있음

* font- weight


>> 폰트 굵기, bold or 100 ~ 900 중의 숫자를 사용할 수 있음
~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <title>실습</title>
      <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">
    <style>
       h1 { text-align: center; }
       h3 { text-align: left; }
       p { text-align: right; }
       #main { width: 50px; }
    </style>
    </head>
    <body>
      <div id="main">
          <h1>가운데</h1>
          <h3>왼쪽</h3>
          <p>오른쪽<p>
    </body>
  </html>
</div>
~~~

>> 자기 자신을 기준으로 정렬이 됨

* line-height

>> 문장 사이의 간격을 조정함

>> 기본은 16

~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <title>실습</title>
      <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">
    <style>
       #up {
           background-color: skyblue;
           line-height: 24px;
           }
    </style>
    </head>
    <body>
      <div id="main">
          <p id="up">ㄹㅇ</p>
    </body>
  </html>
</div>
~~~

* letter-spacing

>> 글자와 글자 사이의 간격을 조정함, 자간

~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <title>실습</title>
      <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">
    <style>
       #up {
           background-color: skyblue;
           line-height: 24px;
           letter-spacint: 5px;
           }
    </style>
    </head>
    <body>
      <div id="main">
          <p id="up">ㄹㅇ</p>
    </body>
  </html>
</div>
~~~

* text-indent

>> 문단의 시작부에 들여쓰기를 함

>> 예시 text-indent: 15px;

