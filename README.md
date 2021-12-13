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
   
### TDD의 이점

- TDD로 많은 기능을 테스트하기 때문에 소스 코드에 안정감이 부여된다.   
- 실제 개발하면서 많은 시간이 소요되는 부분은 디버깅 부분이기에 TDD를 사용하면 디버깅 시간이 줄어들고 실제 개발 시간도 줄어든다.   
- 소스 코드 하나하나를 더욱 신중하게 짤 수 있기 때문에 깨끗한 코드가 나올 확률이 높다.

### React Testing Library

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

# `npm run build`

