# 5강

## 멀티미디어와 관련된 태그

### 이미지 태그

*img
>> <img src="이미지 url" alt="사진 설명" >, 종료 태그가 없음

>> src라는 속성은 source의 약자

>> alt라는 속성은 불러올 이미지가 없거나 불러오는데 실패했을 경우 대신 표시되는 문장

>> weight, height 속성은 이미지의 너비와 높이를 지정할때 쓰는 속성, css에서 조장하는 것을 권장

~~~~
<div>
 <!DOCTYPE html>
 <html>
   <head>
     <meta charset="utf-8">
     <title>실습</title>
   </head>
   <body>
     <img src="data:image/jpeg;base64,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" src="chi0mchak" height="320px" width="150px">
     <iframe width="560" height="315" src="https://www.youtube.com/embed/2kcm_akkCRw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
   </body>
 </html>
</div>
~~~~~~

### 유튜브 영상 넣는 법
>> 영상 공유 --> 퍼가기 --> 복사, 붙여넣기

# 6강

## 테이블
>> th, td, tr 요소로 이루어짐

* table = 표 전체를 감싸는 태그

* tr = 표에서 행을 구분하는 태그

* th = 표의 행 내부에 제목 셀을 담는 태그

* td = 표의 행 내부에 데이터 셀을 담는 태그

>> tr 태그를 기준으로 만들 것.

~~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
       <meta charset="utf-8">
       <title>실습</table>
    </head>
    <body>
      <table>
        <tr>
          <th>성별</th>
          <td>남</td>
          <td>여</td>
        </tr>
        <tr>
          <th>학년</th>
          <td>3</td>
          <td>3<td>
        </tr>
        <tr>
          <th>이름</th>
          <td>수노</td>
          <td>곽두팔</td>
        </tr>
      </table>
    </body>
  </html>
</div>
~~~~

* rowspan

>> rowspan="숫자" "숫자"만큼 셀이 행을 점유

>> ex) <td rowspan="2">3</td>

* colspan

>> colspan="숫자", "숫자"만큼 셀이 열을 점유

## 목록(리스트)

### 순서 없는 목록

* ul
>> 리스트에 항목을 감싸는 태그

* li
>> 리스트에 나열할 항목을 담아두는 태그

### 순서 있는 목록

* ol
>> 리스트에 항목을 감싸는 태그

* li
>> 리스트에 나열할 항목을 담아두는 태그

>>리스트는 기본적으로 들여쓰기를 브라우저 내에 포함하고 있음

## 목록과 관련 있는 속성

### ol 태그 속성

* start

>> 리스트가 시작하는 숫자를 정함

* type

>> 순서를 시작하는 문자를 정함

* reversed

>> 순서를 반대로 시작, 다른 속성과 달리 키만 써서 사용

### list 태그 속성

* value

>> 해당하는 리스트 아이템의 번호를 지정

~~~~
<div>
  <!DOCTYPE html>
  <html>
    <head>
      <meta charset="utf-8">
      <title>실습</title>
    </head>
    <body>
      <h3>리스트</h3>
      <ol type="i">
        <li>밥 먹기</li>
        <li value="3">TV 보기</li>
        <li>운동하기</li>
      </ol>
     </body>
   <html>
</div>
~~~~~~
