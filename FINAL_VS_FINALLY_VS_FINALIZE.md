1.	final, finally, finalize
# final 
## 선언부에 따라 다르다
## class 의 final 사용 - class 가 상속되지 않도록 하기 위하여 선언
## method 의 final 선언 - 상속 관계에 있는 상위 class 와 하위 class 에서 상위 class 에 있는 method 가 재정의(overriding) 되지 않도록 하기 위하여 정의
## variable(변수) 의 final 선언 - 초기 값이 변경되면 안되거나 변경할 경우 예외가 발생할수 있는 경우 사용

# finally
## finally는 try-catch 블록 뒤에 둘 수 있는 선택적인 블록, try-catch문이 끝나기 전에 항상 꼭 실행되어야 하는 로직이 있을 경우 finally절에 작성한다
## 흔한 사용 예로 database connection pool 구현 시, connection과 PreparedStatement 를 클로징 해 줄 때 사용하기도 한다.

# finalize
## java garbage collector가 더 이상의 참조가 존재하지 않는 객체를 발견한 순간 호출하는 메서드
## java.lang.Object클래스로 부터 상속받아 모든 클래스의 객체가 가지고 있는 메서드
## 객체가 삭제되기 직전에 실행되어야 하는 로직같은게 있으면 Object 클래스에 정의된 finalize() 메서드를 오버라이딩하여 정의
## But, finalize()는 언제 호출될지 알 수 없기 때문에, 여기에 의존하는 방식의 구현은 바람직하지 않다.
