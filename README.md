# 테스트 주도 개발(Test Driven Development)

`테스트 주도 개발(TDD)`은 소프트웨어를 개발하는 여러 방법론 중 하나이다.   
제품이 오류 없이 정상 작동하는지 확인하기 위해 모든 코드는 프로그래머가 작성하고 나서 테스트를 거치게 된다.   
TDD에서는 제품의 기능 구현을 위한 코드와 별개로, 해당 기능이 정상적으로 움직이는지 검증하기 위한 테스트 코드를 작성한다.   
이를 통해 테스트가 실패할 경우, 테스트를 통과하기 위한 최소한으로 코드를 개선한다.   
최종적으로 테스트에 성공한 코드를 리팩토링 하는 과정을 거친다.   
   
## TDD 절차

실제 코드를 작성하기 전에 테스트 코드를 먼저 작성한다.   
테스트 코드를 작성한 후, 그 테스트 코드를 Pass할 수 있는 실제 코드를 작성한다.   
   
![TDD 절차](https://user-images.githubusercontent.com/46395776/145811720-522bd17b-002c-4147-830b-ceedd1f25520.png)   
   
## TDD의 이점

- TDD로 많은 기능을 테스트하기 때문에 소스 코드에 안정감이 부여된다.   
- 실제 개발하면서 많은 시간이 소요되는 부분은 디버깅 부분이기에 TDD를 사용하면 디버깅 시간이 줄어들고 실제 개발 시간도 줄어든다.   
- 소스 코드 하나하나를 더욱 신중하게 짤 수 있기 때문에 깨끗한 코드가 나올 확률이 높다.   
   
# React Testing Library

React Testing Library는 React 구성 요소 작업을 위한 API를 추가하여 DOM Testing Library 위에 구축된다.   
DOM Testing Library란 DOM 노드(Node)를 테스트하기 위한 매우 가벼운 솔루션이다.   
   
Create React App으로 생성된 프로젝트는 즉시 React Testing Library를 지원한다.   
그렇지 않고 처음부터 뼈대를 만들어 프로젝트를 생성한다면 다음과 같이 npm을 통해 추가할 수 있다.   
   
`npm install --save-dev @testing-library/react`   
   
# Jest

FaceBook에 의해서 만들어진 테스팅 프레임워크이다.   
최소한의 설정으로 동작하며, Test Case를 만들어서 애플리케이션 코드가 잘 돌아가는지 확인해준다.   
단위(Unit) 테스트를 위해서 이용한다.   
   
## 시작하기

1. Jest 라이브러리 설치 : `npm install jest --save-dev`   
2. Test 스크립트 변경 : `"test": "jest" or "jest --watchAll"`   
3. 테스트 작성할 폴더 및 파일 기본 구조 생성   
   
![jest](https://user-images.githubusercontent.com/46395776/145813919-e561dce2-0198-4225-9507-9446a453fa0f.png)   
   
# Simple App 소개

![simple app](https://user-images.githubusercontent.com/46395776/145814490-392aca19-133d-4a0d-8d04-8df717c9784b.png)   
   
+, -, 그리고 on/off의 버튼이 있다.   
거기서 + 버튼을 누르면 숫자가 올라가고 -를 누르면 내려간다.   
처음 숫자는 0부터 시작한다.   
그리고 on/off 버튼을 누르면 +, - 버튼이 disabled 된다.   
이러한 요구사항을 만족하는 테스트 코드를 작성한다.