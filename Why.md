1. 수정, 삭제 API의 request를 어떤 방식으로 사용하셨나요? (param, query, body)
 - 주소의 변수를 받아와 조회할수있게 만들었다 (Path Variable)
 - ex) /post?post_id=2 이후의 부분을 query string이라고 하며 뒤는 key, value의 쌍으로 이루어집니다.
      다음과 같이 &로 연결하여 여러 개의 데이터를 넘길 수도 있습니다.
 - body는 XML, JSON, Multi Form 등의 데이터를 담는다. 당연히 주소에선 확인할 수 없다.

2. 어떤 상황에 어떤 방식의 request를 써야하나요?
 - Param : 주소의 변수를 받아와야 할때
 - query : 정렬이나 필터링이 필요한 경우
 
 
3. RESTful한 API를 설계했나요? 어떤 부분이 그런가요? 어떤 부분이 그렇지 않나요?
 -URI에 정보의 자원을 표현하였다
 -POST , GET ,PUT , DELETE의 메소드를통해 CRUD를 작성하였다.
 
4. 적절한 관심사 분리를 적용하였나요? (Controller, Repository, Service)
 - 클라이언트에ㅓ 컨트롤러로 요청을받고 서비스에서 레파지토리 순서로 요청을 받을수있게 작성하였다
  
5. 작성한 코드에서 빈(Bean)을 모두 찾아보세요!
 - 컨트롤러에 7개, 서비스에 1개 레파지토리에 1개가 등록되어 관리 되었다
 
8. API 명세서 작성 가이드라인을 검색하여 직접 작성한 명세서와 비교해보세요!(Use Case도 같이있음)
 - https://www.figma.com/file/sf9LiKKQl3tFUFgCikbhOh/Untitled?node-id=0%3A1
