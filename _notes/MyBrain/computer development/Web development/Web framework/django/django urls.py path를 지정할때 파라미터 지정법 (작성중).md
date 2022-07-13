### Date : 2022-06-15 16:02

### Topic : django urls.py path를 지정할때 파라미터 지정법
---
### Summary
> 

#### Content :
- path('user/<int:id>', views.user_info_by_id) 에서 <>는 경로파라미터의 시작과 끝을 의미한다. 경로주소의 사이에 변수값:표시될 변수명으로 입력하면 끝 (일종의 예약어)
- ex) path('user/<str:email>')
- email은 views에 전달될 변수의 이름이 되시겠다. 사용자가 정하는 값이며 urls에서 먼저 정하는 값이다. 가독성만 생각해서 작명하면 되겠다.
- 

### Reference
- 

### Link
-
