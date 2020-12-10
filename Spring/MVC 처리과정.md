------

# 스프링 MVC

------

## ***\*💡\** 스프링 MVC의 기본사상 **

![image](https://user-images.githubusercontent.com/52389219/101736749-3bdbc300-3b07-11eb-9c85-c8f42ed46edb.png)
<BR>
● SERVLET/JSP에서는 HttpServletRequest/HttpServletResponse라는 타입의 객체를 이용해서 브라우저에서 전송한 정보를 처리하는 방식입니다.<br>
● 스프링 mvc의 경우 위의 사진처럼 하나의 계층을 더한 형태가 됩니다.  <br>
● 스프링 MVC를 이용하게 되면 개발자들은 직접적으로 HttpServletRequest/HttpServletResponse 등과 같이 서블릿/JSP의 API를 사용할 필요성이 현저하게 줄어듭니다. <br>
● 스프링 MVC는 내부적으로 SERVLET/JSP 처리를 하니깐 중간에 연결역할을 함으로써 이러한 코드를 작성하지 않고도 원하는 기능을 구현할 수 있게됩니다. <br>

<h5> Model,view and controller </h5>
● model : 데이터를 처리하는 부분을 의미합니다.<br>
● view : 화면을 담당하는 부분입니다.<br>
● Controller : 요청을 처리하는 부분으로 뷰와 모델사이의 통신 역할을 합니다. <br>

<h5> 스프링 MVC의 Controller </h5>
● HttpServletRequest/HttpServletResponse를 거의 사용할 필요없이 필요한 기능 구현 <br>
● 다양한 타입의 파라미터 처리, 다양한 타입의 리턴 타입 사용이 가능합니다. <br>
● GET 방식, POST 방식 등 전송방식에 대한 처리를 어노테이션으로 처리 가능합니다. <br>
● 상속/인터페이스 방식 대신에 어노테이션만으로도 필요한 설정이 가능합니다.<br>

<h6> @Controller 와 @RequestMapping </h6>
● @Controller는 자동으로 스프링의 객체(Bean) 으로 등록되는데 servlet-context.xml에서 스캔하는 코드때문에 그 스캔과정을 통해 자동등록된다. <br>
● @RequestMapping은 현재 클래스의 모든 메서드들의 기본적인 URL경로가 됩니다. <br>
● @RequestMappong은 속성을 추가할 수 있습니다. 가장 많이 사용하는 속성이 method 속성입니다. Method 속성은 흔히 GET방식, POST 방식을 구분해서 사용할 때 이용합니다. <br>
● @Controller 를 작성 할 때 가장 편리한 기능은 파라미터가 자동으로 수립되는 기능입니다. request.getParameter()를 이용하는 불편함을 없앨수있습니다. <br>

자세한 내용은 dispatcherServlet 게시글에서 정리.

# Referece

● 코드로 배우는 스프링 웹 프로젝트 - 구멍가게코딩단

● https://min-it.tistory.com/7
