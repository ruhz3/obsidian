컴퓨터는 크게 `하드웨어`와 `소프트웨어`로 나눌 수 있고, 
소프트웨어는 크게  `시스템 소프트웨어`와 `사용자 어플리케이션`으로 나눌 수 있다. 

일반적으로 시스템 소프트웨어의 개발 영역은 `Native`라 부른다.
보통 C, C++로 개발되고 [[플랫폼 의존성]]을 갖는다.

사용자 어플리케이션은 시스템 소프트웨어 위에서 프로세스로서 동작한다.
논리적(Logical = `Virtual`)으로 하드웨어(CPU = `Machine`)를 구현한 사용자 어플리케이션 레벨의 프로세스이며, 인식할 수 있는 코드가 `Java` 바이트 코드인 것을 "Java Virtual Machine" 이라고 한다.

여기서 하드웨어는 `Machine` 꼭 CPU 뿐 아니라, RAM, SSD도 가상 메모리로 추상화하고 있다.
여기에 OS의 일부 기능까지 JVM에서 제공한다. 

(즉, JVM을 완벽히 이해하고 싶다는 이야기는,,, 이 모든 것을,,,)

아무튼 JVM은 이 모든 것은 사용자 어플리케이션 영역으로 가져왔기 때문에,
장애나 에러가 발생해도, 직접적으로 OS 레벨의 영향을 주기는 어렵다. (JNI?)
