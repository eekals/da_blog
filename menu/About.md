<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>나만의 웹페이지</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f9;
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    h1 {
      text-align: center;
      margin-top: 20px;
      color: #333;
    }
    h2 {
      margin-left: 20px;
      color: #555;
    }
    ul, ol {
      margin-left: 40px;
    }
    table {
      width: 80%;
      margin: 20px auto;
      border-collapse: collapse;
    }
    table, th, td {
      border: 1px solid #ddd;
    }
    th, td {
      padding: 10px;
      text-align: left;
    }
    form {
      width: 80%;
      margin: 0 auto;
      padding: 20px;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    label {
      display: block;
      margin: 10px 0 5px;
    }
    input[type="text"], textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      border: 1px solid #ddd;
      border-radius: 4px;
    }
    input[type="submit"] {
      background-color: #4CAF50;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    input[type="submit"]:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>

  <!-- 제목 -->
  <h1>Ohdamin's Webpage</h1>

  <!-- 자기소개 테이블 -->
  <h2>자기소개</h2>
  <table>
    <tr>
      <th>항목</th>
      <th>내용</th>
    </tr>
    <tr>
      <td>이름</td>
      <td>Ohdamin</td>
    </tr>
    <tr>
      <td>나이</td>
      <td>25</td>
    </tr>
    <tr>
      <td>관심사</td>
      <td>데이터 분석, 웹 개발, 인공지능</td>
    </tr>
    <tr>
      <td>사용 툴</td>
      <td>Python, R, SQL</td>
    </tr>
  </table>

  <!-- 좋아하는 것 및 취미 목록 -->
  <h2>나의 취미와 기술 스택</h2>
  <ul>
    <li>데이터 분석</li>
    <li>웹 개발</li>
    <li>인공지능</li>
    <li>책 읽기</li>
    <li>영화 감상</li>
  </ul>

  <!-- 방문자가 메시지를 남길 수 있는 폼 -->
  <h2>방문자 메시지 남기기</h2>
  <form action="#" method="POST">
    <fieldset>
      <legend>메시지 폼</legend>
      
      <label for="name">이름</label>
      <input type="text" id="name" name="name" placeholder="이름을 입력해주세요">
      
      <label for="message">메시지</label>
      <textarea id="message" name="message" rows="4" placeholder="남기고 싶은 메시지를 작성해주세요"></textarea>
      
      <input type="submit" value="메시지 보내기">
    </fieldset>
  </form>

</body>
</html>
