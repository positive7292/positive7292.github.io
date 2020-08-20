# 7강

* form 태그

>> 폼에 포함되는 다양한 입력 양식 태그들을 감싸줌

## 폼 속성

* action

>> 데이터를 보낼 URL을 지정

>> 해당 데이터를 처리할 웹 서버 URL을 담고있음

* method

>> 보내는 방식을 지정

>> 값으로는 get, post가 있음

>> 폼에 입력한 데이터를 서버로 보내는 역할

>> 서버로 데이터를 보낼 때 메시지에 담아서 보냄

>> 그 메시지를 HTTP Request Message라고 부름

>> 메시지는 header와 body로 구분이되는데 header 부분에 목적지 서버 url을 적음

* method="get" 방식

>> 브라우저에서 폼에 입력한 데이터를 url 끝에 붙여 눈에 보이게 보냄

>> 데이터 조회 만을 목적으로 할 때 주로 쓰임 ex> 검색

* method="post" 방식

>> 데이터를 메시지의 body 부분에 숨겨서 보냄

>> 서버에 있는 데이터를 쓰거나 수정, 삭제할 때 주로 사용 ex> 게시물 작성

## input

>> 사용자에게 입력을 받기 위해 사용되는 태그, 빈 태그

>> 종류가 워낙 다양해 다양한 용도로 사용 가능

>> type과 name 이라는 속성이 있음

>> 예시 input type="text" name="id"

* placeholder 속성

>> input에 아무 값도 입력 되지 않았을 때 나타나는 텍스트

* value 속성

>> 서버로 데이터를 전송할 때 들어가는 값과 동일함

>> 사용한다면 초기값으로 값이 들어감

## label

>> 폼이 어떤 역할을 하는지 알려주는 이름표와 같은 역할을 함

>> for 속성과 함께 입력이 됨

>> input 태그 앞에 들어감

## div 

>> 태그들을 구분 짓고 나누기 위해 사용되는 태그

## select

>> 미리 준비된 여러 개의 선택지를 선택하게 하는 선택 박스

>> select 태그와 하위의 option 태그로 이루어짐

>> name이라는 속성을 반드시 가져야 함, input의 name과 동일

>> 각 option 태그는 value라는 속성을 반드시 가져야 함

## textarea

>> 한 번에 많은 글을 입력 받을 때 사용, 긴 글

>> cols는 폭, rows는 높이

## button

>> html 요소를 버튼 내부에 담을 수 있어 유용함

>> 이미지 버튼의 제작이 가능함

~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <title>실습</title>
    </head>
    <body>
      <h2>회원가입</h2>
      <form action="URL삽입" method="get">
         <div>
           <label for="userid">아이디: </label>
           <input type="text" name="id" placeholder="아이디를 입력하세요." value="snow">    
         </div>
         <div>
           <label for="password">비밀번호: </label>
           <input type="password" name="password" placeholder="비밀번호를 입력하세요"> 
         </div>
         <div>
            <label for="gender">성별: </label>
            <select name="gender" id="gender">
               <option value="male">남성</option>
               <option value="female">여성</option>
            </select>
         </div>
         <div>
            <label for="job">직업: </label>
            <select name="job id="job>
               <option value="student">학생</option>
               <option value="teacher">선생님</teacher>
               <opation value="etc">기타</
            </select>
         </div>
         <div>
            <label for="introduct">자기소개: </label>
            <textarea name="introduce" id="introduce" cols="30" rows="10 placeholder="자기소개를 입력하세요">
         </div>
         <button type="submit">제출</button>
         <button type="reset">리셋</button>
      </form>
    </body>
  </html>
</div>
~~~

