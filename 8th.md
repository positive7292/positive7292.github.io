# 8강

## CSS(style sheets)

~~~
<div>
  선택자p{
    속성font-family: 값'맑은 고딕';
    속성font-size: 값18px;
    속성color: 값blue;
    }선언 블록 {}로 분류
</div>
~~~

### 선택자

>> 스타일을 적용하고자 하는 html 요소를 선택하는 역할

### 속성

>> 지정할 스타일의 속성명에 해당 속성: 값;이 한 단위

### 값

>> 키워드나 특정 단위를 사용하여 원하는 스타일을 적용, 속성과 짝을 이룸

* css는 html에 적용해야 사용이 가능

## html을 css에 적용하는 방법

### link style
>> html 외부에 있는 css 파일을 불러옴

>> head 태그 사이에 link 태그를 추가시켜줌

>> ex) 
~~
<link rel="style sheet" href= "text.css">
~~

### embedding style
>> html의 <head>에 <style>을 이용하여 css를 작성

~~~
 <style>
   h1 { color: red;}
 </style>
~~~

### inline style

>> html 요소에 직접 style 속성을 이용하여 css를 작성

~~~
 <h1 style="color: red;"></h1>
~~~

# 9강

## 선택자
>> 스타일을 적용하고자 하는 html 요소를 선택하는 역할

>> 일반적인 태그를 선택자로 사용할 수 있음

>> 중복되는 코드를 막기 위해서는 여러 개의 선택자를 ,를 이용해 한꺼번에 지정 가능

* 타입 선택자
>>해당 태그를 가지는 모든 요소에 선택자를 적용

* 아이디 선택자
>> id로 스타일을 적용, 해당 id 하나에 적용

>> id는 다른 요소와 구분점을 만들어줌

>> #과 지정 아이디를 사용

* 클래스 선택자
>> 클래스는 비슷한 특징을 갖는 요소를 지정하여 묶을 수 있음

>> 클래스 이름으로 스타일을 적용, 같은 클래스 이름이면 모두 적용

* 전체 선택자
>> 간단히 모든 요소에 스타일을 적용, 속도가 저하될 수 있어 쓰지않기를 권장

>> 선택자의 자리에 *을 사용

* 속성 선택자
>> 특정 속성을 소유하는 모든 요소에 스타일을 적용

>> 선택자[속성명="속성값"] { color : red; }

~~~
<div>
<!DOCTYPE html>
<html>
   <head>
     <title>실습</title>
     <style>
        p { color: red; }   타입 선택자
        h2 { color: blue; } 타입 선택자
        #snow { background-color: yellow; }  아이디 선택자
        .contents { font=size: 24px; }
     </style>
   </head>
   <body>
     <h1>원석</h1>
     <p>1단락</p>
     <h2 id="snow">작은 단락</h2>       아이디 선택자
     <p class="contents">두번째 단락</p> 클래스 선택자
     <h2>작작은 단락</h2>
     <p class="contents">세번째 단락</p> 클래스 선택자
   </body>
</html>
</div>

   <head>
     <title>실습</title>
     <style>
        a[target="_blank"] { color: red; } 속성 선택자
     </style>
   </head>
   <body>
     <a href="" target="_self">구글 현재창</a>
     <a href="" target="_blank">구글 새 창</a>
     <a href="" target="_self">구글 현재창</a>
   </body>
~~~

## 복합 선택자

* 자식 선택자
>> 선택자a의 모든 자식 중 선택자b와 일치하는 요소를 선택

>> 선택자a > 선택자b{color : red;}

>>  예시 article > p{color : red;}

* 후손 선택자
>> 선택자 a의 모든 후손 중 선택자b와 일치하는 요소를 선택

>> 선택자a 선택자b {color: blue;}

>> 예시 article p {color: blue;}

## pseudo 선택자

* pseudo 클래스
>> 요소의 특별한 상태를 지정할 때 씀

>> 가상의 클래스

>>> :link 방문하지 않는 상태일 경우
>>> :visited 방문한 링크일 경우
>>> :hover 요소에 마우스가 올려져 있을 경우

~~~
   <head>
     <title>실습</title>
     <style>
        a:link { color: yellow; }  peusdo 선택자
     </style>
   </head>
   <body>
     <a href="">구글 현재창</a>
   </body>
~~~
