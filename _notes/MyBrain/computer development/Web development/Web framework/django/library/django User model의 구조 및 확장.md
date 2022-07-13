### DATE : 2022-07-05 12:26
# Topic : django User model의 구조 및 확장

### comment
> django에서는 회원정보를 관리할 수 있는 기능을 재공하고, 이 앱의 이름은 django.contrib.auth 이다. 여기의 User모델을 활용해서 회원관리 및 여러 인증을 구현할 수 있다.

### 지원되는 User Field list
- username (<=150, incudel[_, @, +, ., - ] )
- first_name (<=150)
- last_name (<=150)
- email(blank=True)
- password
- groups
- user_premissions
- is_staff (True or False)
- is_active (True or False)
- is_superuser (True or False)
- last_login (datetime)
- date_joined (datetime)


### Link :
- django.contrib.auth Documentation 참조 [https://docs.djangoproject.com/en/4.0/ref/contrib/auth/]
- 