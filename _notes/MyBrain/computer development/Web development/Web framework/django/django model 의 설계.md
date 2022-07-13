### Date : 2022-06-15 16:02

### Topic : django model 의 설계
---
### Summary
> django의 MTV 패턴에 따르면, M은 Model로, 장고가 구성할 웹 서비스의 Database 에 들어갈 Table의 record를 설계한다.

#### Content :
- 대부분의 모델은 Models class를 파생받아야한다.(왜?인지 생각해볼것)
- class Models에는 사용자 편의를 위해 지정해둔 많은 모델들이 있으며, 파생시 이를 사용할 수 있다.
- DateTimeField(auto_now_add=True, null=False)
- CharField(max_length=50, null=False)
- ForeignKey(Topic, on_delete=models.CASCADE
- ForeignKey 의 경우 연결된 record가 삭제될 경우, on_delete의 유형에 따라 데이터가 수정된다.
- on_delete의 유형에는 CASCADE, SET_NULL, DO_NOTHING 등이   있으며, 같이 지워지게 할 것인지, 참조만 끊어지게 할 것인지를 결정할 수 있다.
- 특정 model을 추가한 이후에는 설계한 model을 실제 RDBMS로 스키마를 동기화 하는 작업을 해야함.
- 동기화작업을 위해 python manage.py makemigrations 라는 명령어를 입력해야함
- 정확히는 스키마 변경이 생길 때 마다 마이그래이션을 해야함.
- 마이그래이션이 끝나면, 해당 스키마를 실제 DB에 적용하기 위해서 python manage.py migrate 을 입력해야함.
- Topic.object.get(?)은 객체에서 특정 데이터 1개를 당겨올 때 쓸 수 있다.
- Option.objects.filter(topic=topic).all() 에서 filter()는  특정 조건과 일치하는 레코드를 탐색한다.
### Reference
- 

### Link
-
