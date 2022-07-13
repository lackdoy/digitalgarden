### Date : 2022-06-15 16:02

### Topic : django csrf_token 역할
---
### Summary
> csrf(Cross Site Request Forgery)의 약어로, Post의 요청을 보낼때 해커의 해킹요청을 방어하기 위한 수단으로, 해커가 유추하기 어려운 무작위 값을 생성한 뒤 form 요청을 보낼때 같이 전송되도록 하고 서버에서 이 값이 정상적으로 같은값인지를 확인해서 유효한 데이터인지를 식별하기 위한 방법이다.

#### Content :
- 만약 POST를 처리할 때 csrf 토큰의 값이 폼의 단계에서 돌아오지 않는다면, 정상적인 요청이 아님으로 인식하여 방어로직이 작동함.
- Cross site attack을 막기 위한 방어기제
- 

### Reference
- 

### Link
-
