# 회원가입 창 만들기

![image1](https://user-images.githubusercontent.com/74912530/138545992-5d81fc05-4a9d-4da8-93b0-ca9c9b543e5c.png)
<br>
HTML, CSS, JavaScript를 이용해서 간단한 회원가입 폼을 만들어 보았습니다. 폼을 제작하고 자바스크립트로 형식 체크라던가, 커서이동, 에러표시, 문자인증 토큰발행과 인증확인, 버튼의 활성화, 비활성화와 같은 DOM조작을 하였습니다.

### <웹호스팅 링크>
https://k-junyyy.github.io/SIGN-UP-PAGE/signup.html
<br><br><br>

## 🔨 구현한 기능 

✔️ 맨 처음 disabled 속성을 주어 인증번호 전송, 인증 확인, 가입하기 버튼 클릭 방지

✔️ 지역 선택란에서 초기값은 "지역을 선택하세요"로 하며, "지역을 선택하세요"는 선택 불가

✔️ 성별은 남성, 여성 둘 중 하나만 선택 가능

✔️ 휴대폰 번호 입력 시 3자리, 4자리, 4자리로 입력할 수 있도록 구현

✔️ 첫째 칸 3자리 입력 시 둘째 칸으로 포커스(커서) 이동

✔️ 둘째 칸 4자리 입력 시 셋째 칸으로 포커스(커서) 이동

✔️ 셋째 칸 4자리 입력 시 인증번호 전송 버튼 활성화

✔️ 인증번호 전송 버튼 클릭 시 토큰 생성 및 타이머 실행, 인증 확인 버튼 활성화

✔️ 3분 이내 인증 확인 버튼 클릭 시 "인증이 완료되었습니다" 알림 띄우기

✔️ 3분 동안 버튼을 누르지 않는 경우 인증번호 전송 버튼과 인증 확인 버튼 비활성화

✔️ 문자인증 후 토큰 정보를 "000000", 시간을 "03:00"으로 초기화

✔️ 인증 확인 시 인증 확인 버튼을 "인증 완료"로 변경, 가입하기 버튼 활성화

✔️ 가입하기 버튼 클릭 시 이메일, 이름, 비밀번호, 비밀번호 확인, 지역, 성별 확인

✔️ 가입 시 이메일 형식("아이디"+@+"서버")을 준수하는지 판별

✔️ 가입 시 비밀번호와 비밀번호 확인이 일치하는지 비교

✔️ 가입 시 각 입력창에서 조건에 맞지 않는다면 입력창 아랫부분에 빨간 글씨로 에러 표시

✔️ 조건을 모두 만족시키고 가입하기 버튼  클릭 시 입력창 아래 에러 제거 후 가입 확인 메시지 띄우기
<br><br><br>


![image2](https://user-images.githubusercontent.com/74912530/138545988-31b6d280-18e4-4247-967e-f354dcfe20e9.PNG)
<br>
전화번호 부분(3자리, 4자리, 4자리) 입력 시 인증번호 전송 버튼이 활성화됩니다.
<br><br>

![image3](https://user-images.githubusercontent.com/74912530/138545989-191a6078-00f4-481b-8b8d-f8d33fbf14fb.PNG)
<br>
인증번호 전송 버튼 클릭 시 토큰이 발행되고 3분의 제한시간이 주어집니다.
(아래의 코드에선 빠르게 테스트해보기 위해 1초를 50ms로 설정하였습니다.)
인증확인 버튼을 클릭하면 인증번호전송 버튼과 인증확인 버튼이 비활성화 되고 
인증확인 버튼의 값이 "인증완료"로 바뀌게 됩니다.
<br><br>

![image4](https://user-images.githubusercontent.com/74912530/138545990-276cad02-335a-4417-a35e-0e2afd251123.PNG)
<br>
가입하기 클릭 시 위와같이 이메일 형식이 맞지 않는다거나 이름 누락, 비밀번호와 비밀번호확인이 일치하지 않음, 지역 미선택, 성별 미선택 등등 입력이 올바르지 않다면 빨간 글씨로 에러를 표시해줍니다.
<br><br>

![image5](https://user-images.githubusercontent.com/74912530/138545991-a126e5da-1c81-4fb8-99d1-93a09c9d25a0.PNG)
<br>
형식을 올바르게 입력하고 가입하기 버튼을 클릭하면 가입이 완료되었다는 메시지를 표시하도록 하였습니다.
<br><br>

<div align=center><h1>📚 STACKS</h1></div>
<div align=center> 
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> 
  <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black">
</div>
