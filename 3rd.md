# 링크 태그

* a 태그
>> 닻과 같은 역할을 함

>> <a>태그에는 다른 태그와는 달리 속성이라는 특성이 필수적으로 들어감


>> 속성은 시작태그 괄호 안에 들어감

>> 속성이란 태그의 특징을 뜻함. 태그에 대한 추가적인 정보를 제공

>> <a 키="링크주소">설명</a>

*href 
>> 연결할 웹사이트 주소를 담는 속성

~~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
       <meta charset="utf-8">
       <title>세번째실습</title>
    </head>
    <body>
      <a>구글</a>
      <a href="www.google.com">구글</a>
      <a href="www.daum.net">다음</a>
    </body>
  </html>
~~~~
  
#경로
>>  목적지까지 가는 모든 길

>> 프로그래밍에서 경로는 /를 통해서 표시

>> 주소 + 경로 = URL

#URL
>>웹에서 HTML페이지, CSS문서, 이미지 등 자원의 위치를 나타냄

>> 절대 URL : 접근하는 최초 시작점부터 경유한 경로를 모두 기록하여 리소스의 위치를 나타냄

>> 예시 : http://myblog.com/about/myface.jpg

>> 상대 URL : 기준점을 기준으로 상대적인 경로를 기록하여 리소스의 위치를 나타냄, 내 위치를 기준

>> 예시 : http://about/myface.jpg   <--- 내 위치가 myblog.com 

#target
>> 링크를 열 때 어디에 오픈할 것인지를 정하는 속성

*_self
>> 현재 탭에서 링크를 여는 속성

*_blank
>> 새 탭(창)에서 링크를 
