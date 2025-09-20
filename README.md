# DOCTYPE

HTML 파일에서, doctype(문서 유형 선언)은 모든 문서 맨 위에 위치한 필수적인 <!doctype html> 선언이다.

이 선언의 유일한 목적은 브라우저가 문서를 렌더링 할 때 "쿽스 모드(quirks mode)"로 전환되는 것을 방지하는 것이다.

다시 말해서 <!doctype html> 선언은 브라우저가 관련된 표준 사양을 최대한 따라 렌더링 하도록 보장하며, 일부 사양과 호환되지 않는 다른 렌더링 모드를 사용하지 않도록 한다.

Doctype은 대소문자를 구분하지 않는다. MDN(Mozilla Developer Network)의 코드 예제에서는 소문자를 사용하는 것이 관례이나, <!DOCTYPE html> 처럼 대문자로 작성하는 경우도 흔하다.

<br>

## 쿽스 모드(Quirks Mode)와 표준 모드(Standards Mode)의 이해

웹의 초창기에는 웹 페이지를 두 가지 버전으로 작성하는 것이 일반적이었다. 하나는 Netscape Navigator용, 또 하나는 Microsoft Internet Explorer 용이었다. 이후 W3C에서 웹 표준을 제정했으나 브라우저들은 이를 곧바로 적용할 수 없었는데, 그렇게 하면 기존 웹사이트들의 대부분이 제대로 작동하지 않기 때문이었다.

그래서 브라우저들은 **새로운 웹 표준을 따르는 사이트와 기존 방식의 레거시 사이트** 를 다르게 처리하기 위해 **두 가지 모드** 를 도입하게 되었다.

현재 웹 브라우저의 레이아웃 엔진(layout engine)은 다음 **세 가지 모드**를 사용한다 :

1. 쿽스 모드 (Quirks Mode)

   - 레이아웃 동작이 Netscape Navigator 4와 Explorer 5의 동작을 모방한다.

   - 웹 표준이 널리 채택되기 전에 만들어진 기존 사이트들을 지원하기 위해 꼭 필요하다.

2. 리미티드 쿽스 모드 (Limited-Quirks Mode)

   - 아주 **소수의 예외(quirk)** 만 적용된 모드이다.

3. 표준 모드 (No-Quirks Mode)

   - HTML 과 CSS의 최신 웹 표준 명세에 따라 동작한다.

   - 의도된 대로의 정확한 동작이 기대되는 모드다

<br>

## Netscape Navigator

Netscape Navigator(또는 간단히 Netscape)는 1990년대에 가장 널리 사용되던 웹 브라우저 중 하나다. 이 브라우저는 Mosaic이라는 초기 웹 브라우저를 기반으로 만들어졌으며 개발 팀은 Mosaic의 개발자였던 **Marc Andreessen(마크 앤드리슨)**이 이끌었다.

Netscape는 웹을 **텍스트 중심에서 그래픽 중심으로 바꾸는 데 큰 역할** 을 했다. 오늘날 표준이 된 많은 브라우징 기능들이 Netscape를 통해 처음 도입되었다. 예를 들어서 웹페이지를 로딩하면서 바로 표시할 수 있었고 **양식(form)**이나 인터랙티브 콘텐츠에 JavaScript를 사용할 수 있었으며 세션 정보를 쿠키에 저장하는 기능도 제공했다.

기술적인 우위와 초반의 시장 지배력에도 불구하고 **1990년대 후반에는 Internet Explorer(인터넷 익스플로러)**가 빠르게 시장 점유율을 넷스케이프보다 더 많이 차지하게 되면서 Netscape는 점점 밀려나게 되었다.

<br>

## Microsoft Internet Explorer

Internet Explorer(또는 IE)는 마이크로소프트(Microsoft)에서 유지 관리하던 그래픽 기반의 무료 웹 브라우저로, 주로 기업 환경의 레거시 시스템에서 사용되었다. 현재는 Microsoft Edge가 윈도우의 기본 브라우저로 자리 잡고 있다.

마이크로소프트는 1995년, **"Microsoft Plus!"**라는 패키지의 일부로 Internet Explorer를 Windows에 처음 포함시켰다. 이후 약 2002년경에는 IE가 전 세계에서 가장 많이 사용되는 웹 브라우저가 되었지만 시간이 지나면서 Chrome, Firefox, Edge, Safari 등의 브라우저에 점점 점유율을 빼앗기게 되었다.

IE는 다양한 버전으로 출시되었고, 데스크톱, 모바일, Xbox 콘솔용으로도 제공되었다. 또한 Mac과 UNIX용 버전도 있었지만 각각 2003년과 2001년에 지원이 중단되었다. Windows용으로 출시된 최종 버전은 11.0.220이며 2020년 11월 10일에 배포되었다.

마이크로소프트는 2022년 6월 15일, Internet Explorer에 대한 공식 지원을 종료했다.
