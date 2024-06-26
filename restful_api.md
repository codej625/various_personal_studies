# RESTful API에 대해 알아보자.

<br /><br /><br />


* Method 별 URI 설계
```
GET: 리소스를 조회.
POST: 새로운 리소스를 생성.
PUT: 기존 리소스를 업데이트.
PATCH: 리소스의 일부를 업데이트.
DELETE: 리소스를 삭제.
```

<br />

1. GET
```
리소스 조회에 대한 URI는 리소스의 식별자를 포함한다.

예시1 -> 모든 사용자를 조회하는 URI /users가 될 수 있고,
예시2 -> 특정 사용자를 조회하는 URI /users/{id}가 될 수 있다.
```

<br />

2. POST
```
새로운 리소스를 생성하는 URI는 기본적으로 해당 리소스의 부모 리소스를 가리키고,
HTTP 메소드는 대개 POST가 된다.

예시 -> 새로운 사용자를 생성하는 URI /users가 될 수 있다.
```

<br />

3. PUT 또는 PATCH
```
리소스를 업데이트하는 URI는 해당 리소스의 식별자를 포함해야 한다.
PUT 메소드는 전체 리소스를 업데이트하는 데 사용되고,
PATCH 메소드는 리소스의 일부를 업데이트하는 데 사용된다.

예시 -> 특정 사용자 정보를 업데이트하는 URI /users/{id}가 될 수 있다.
```

<br />

4. DELETE
```
리소스를 삭제하는 URI는 해당 리소스의 식별자를 포함해야 한다.

예시 -> 특정 사용자를 삭제하는 URI는 /users/{id}가 될 수 있다.
```
