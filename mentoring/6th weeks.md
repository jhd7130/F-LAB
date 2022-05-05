# 6주차 
  
### AOP(관점지향프로그래밍)  
  
  
**Aspect Oriented Programming**
어플리케이션의 코드를 자세히 보면 실행의 흐름에서 사용자의 부분과 개발자 혹은 운영자의 부분이 나눠져있다. 사용자를 위한 로직과 개발자를 위한 로직이 나눠져있다면 주요로직을 이해하는데 방해요소가 사라지기 때문에 더 많은 이해에 도움이 된다.  
  
login 기능, post 기능 등 50개의 기능이 존재한다고 가정해보자. 각각의 기능에는 로그 기능이 존재하지 않는다. 그래서 개발자가 모든 기능에 대해 로그를 볼 수 있게 logging 처리를 하려한다. 그럼 어떻게 해야할까? 단순하게 생각해보면 50개의 기능을 담당하는 객체의 코드를 모두 열고 각각 작성해주면 된다. 자 이제 힘들게 모두 작성을 완료했다. 근데 갑자기 다른 라이브러리를 사용해야한다는 요청이 들어왔다고 하자. 그럼 퇴사를 결정하는 편이 더 좋다고 본다.  

하지만 퇴사할 필요는 없다. AOP를 쓰면된다. 
  
 ### AOP 구현체
 1. Aspect J : 모든 단위에서 사용가능하며 컴파일시기에 반영된다.(더 자세함)
 2. Spring AOP : Method단위에서 사용가능하며 런타임시에 반영된다.(부가적인 기능으로서의 추가 삭제를 지원하기 위함)

Aspect J보다는 먼저 Spring AOP에 대해 알아보자.  

