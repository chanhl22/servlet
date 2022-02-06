# **직접 만든 프레임워크 스프링 MVC 비교**

## **직접 만든 MVC 프레임워크 구조**

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/48e04983-f19a-4015-b305-61a3336d9102/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220206%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220206T125145Z&X-Amz-Expires=86400&X-Amz-Signature=74aa0119060460c73b0ec21786404e4f60268d6b7d09f2cdb0f07d06e3ee0fea&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

## **SpringMVC 구조**

![Untitled](https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F1e8e8339-a4e2-4571-b533-54b8964662a7%2FUntitled.png?table=block&id=ab58a2cc-d3ba-44c4-992a-5a8a0a7a6c34&spaceId=f034e1fe-a8bf-404e-9dd8-7d2ec0a2f3a9&width=1540&userId=3df801ed-a0e9-4f4e-9367-b72fdd17d55d&cache=v2)

## 비교

- FrontController → DispatcherServlet
    - **DispatcherServlet이 가장 중요합니다.**
    - **스프링 MVC에서는 DispatcherServlet가 바로 프론트 컨트롤러 패턴을 구현한 프론트 컨트롤러 입니다.**
- handlerMappingMap → HandlerMapping
    - 스프링은 HandlerMapping를 인터페이스로 만들어서 더 확장성 있게 만들었습니다.
- MyHandlerAdapter → HandlerAdapter
    - 스프링은 HandlerAdapter를 인터페이스로 만들어서 더 확장성 있게 만들었습니다.
- ModelView → ModelAndView
- viewResolver → ViewResolver
    - 스프링은 ViewResolver를 인터페이스로 만들어서 더 확장성 있게 만들었습니다.
- MyView → View
    - 스프링은 View를 인터페이스로 만들어서 더 확장성 있게 만들었습니다.