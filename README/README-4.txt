chromdriver

현재 크롤링은 정해진 url만 처리합니다
이런 상태는 ststic 입니다

dynamic은 payload로 url을 주면 재활용해서 서로 다른 결과를 만드는 것입니다

==========================================================================

MVC 코딩하는 순서
1. model을 만들고 -> view를 만들어서 -> controller로 연결(network)합니다
model = entity + service 속성 + 기능 => 모델 객체
view = Reactjs로 전환됩니다

model과 view가 언어가 다릅니다

python과 javascript(reactjs)는 서로 syntax가 다릅니다
그래서 transfer를 불러서 data를 주고 받을 수 있습니다
flask가 transfer의 역할을 하는데 통역하는 객체의 언어가 python입니다

각각 하는 일이 다릅니다
뇌의 역할을 하는 모델은 python입니다

플젝을 만드는데 칩을 이식하면 단기간에 성능이 올라갑니다
유료칩(스타트업)도 있고 무료칩도 있는데 
이 중 성능이 검증된 유명한 것이 tensorflow((주)Google), pytorch((주)facebook)입니다

코딩 컨벤션을 결국 텐서플로에 최적화 시켜야 합니다
그래서 객체지향(class 단위)방식으로 바꾼 것입니다

인공지능을 담당하는 미세조정 파트는 텐서플로에 의존합니다

이제 구조(뼈대)는 잡았으니 디테일한 파트인 알고리즘으로 넘어갑니다

==========================================================================

machine vs model - difference

컴공 상태를 통해 구분 state
machine은 러닝을 합니다
model은 러닝을 하지 않습니다

우리가 모델을 만듭니다
그런데 모델을 러닝시키는 것이 아니라 
머신을 러닝시킵니다
머신은 학습을 이미 한 객체가 아닌 학습을 할 객체입니다

알고리즘을 공부하는 목적이 머신러닝에서는 머신을 공부시키는 것입니다
머신이 공부해서 내는 performance가 성과입니다

어떤 알고리즘을 우리가 만드는 모델에 주입을 시킬 것인가를 고민해야 합니다

==========================================================================

모델을 만드는 순서

첫번째는 모델을 훈련시킬 데이터에서 쓰레기값은 제거하는 것입니다
이 머신은 타이타닉의 정보를 통해 
만약 A 라는 가상의 인물이 당시 1912년 침몰 당시 타이타닉에 승선했다면 생존확률이 얼마인지
더 나아가 현재 승객 안전을 위한 조치를 어떻게 하면 비슷한 사고 발생 시 생존률을 올릴 수 있는지에
대한 문제로 귀결될 수도 있습니다


우리는 단순하게 생존확률 판단 머신부터 만들겠습니다

1순위 작업은 feature 를 drop 시키는 것입니다