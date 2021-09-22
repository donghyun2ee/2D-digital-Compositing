첫 기터부. 등록
# 2D-Digital-Compositing
## 2D
-------------------
1. 2D의 정의 평소의 우리가 아는 2d란 X, Y축으로 보여지는 그래픽의 요소 하지만 그것은 수학의 정리 이다.  2D 디지털에 관련된 것은 결과 매체가 2D 라는것.
> 디지털 어희
2. Digit: 0~9 까지의 아라비아 숫자
3. Vector: 표현 vector2 (x,y) vector3 (x,y,z) vector4 (x,y,z,w)
4. Integer: 소숫점이 필요없다. 0,1,2,3,4...
5. Float: 0.1, 2.35, 3.142...
6. Boolean: 0(off) or 1(on)  ex 레이어를 껏다 켰다. - 불린데이터 
## Compositing
> Compositing(합성)
1. 둘 이상의 것을 합쳐서 하나를 이룬다.
## Color
컬러란 무엇인가.
> "빛깔" 혹은 "색" 이라는 뜻을 갖고 있다. 빛의 주파수(파장)의 차이에 따라 색상이 다르게 느껴진다.
1. 주요 속성에서는 색상, 채도, 명도가 있다
2. 색상: 빛의 파장과 밀접하다
3. 채도: 빛의 선명도를 나타낸다.
4. 명도: 빛의 밝기를 나타내는 지표이다.
> 삼원색 - 가산혼합과 감산혼합에서 기본이 되는 색이다.
1. ![image](https://user-images.githubusercontent.com/90343486/134352659-357b3f9c-a188-4b2e-9d83-c53b0cdea896.png)
 가산혼합 - R(빨강), G(초록), B(파랑) - 빛의 삼원색 ex) 모니터, 빛, 스크린
2. ![image](https://user-images.githubusercontent.com/90343486/134352790-41d947d4-211f-466b-97d6-a2d561bacb94.png)
 감산혼합 - C(시안), M(마젠타), Y(노랑), K(블랙) - 색의 삼원색 ex) 잉크, 프린트, 인쇄물
3. 출처 https://ko.wikipedia.org/wiki/%EC%83%89
## Alpha
알파란 무엇인가.
> Alpha 채널 
> 알파 채널 또는 알파 합성은 a채널과 이미지 처리 분야에 있고, 각 화소에 대해 색상 표현의 데이터로 보조 데이터를 말한다.
1. Alpha 값은 0.0(완전 투명색) ~ 1.0(완전 불투명) 으로 표현이이 된다.
2. ![image](https://user-images.githubusercontent.com/90343486/134357688-8289b809-ce68-4a40-8c71-52b25d59ed53.png)
3. 출저 https://ko.wikipedia.org/wiki/%EC%95%8C%ED%8C%8C_%EC%B1%84%EB%84%90
## Color space
Color space(색공간) 무엇인가.
> 색공간은 색 표시계(color system)를 3차원으로 표현한 공간의 개념이다. 모든 색들은 이 색 공간에서 3차원 좌표로 나타낸다.
### 색 표시계
1. 색 표시계는 CIERGB, CIEXYZ, CIELAB, CIELUV 등의 색 체계를 말한다.
2. 디자인 학계나 산업계에서 색채 디자인 또는 시각 디자인등 카메라, 스캐너, 모니터, 프린터 등에 사용
3. 컬러 영상 장비 개발 및 응용 단계에서 색 공간은 정확한 색 표현을하기위해 필수적이다.
4. 디지털, 디자인에서 사용되는 색 공간은 CIELAB 색공간이며, 먼셀 색 표시계의 기본 원리 색의 3속성(색상(hue), 명도(Value), 채도(Saturation)를 사용한다.
#### RGB 색 공간
1. 색을 혼합하면 명도가 올라가는 가산 혼합 방식이다. R(레드), G(그린), B(블루) 의 삼원색이 있다.
2. ![image](https://user-images.githubusercontent.com/90343486/134359532-9262ac8b-5205-4dc0-8055-4d747c21ffac.png)
#### CMYK 색 공간
1. 색을 혼합하면 명도가 낮아지는 감산 혼합 방식이다. 인쇄과정에서 쓰이며, 네 가지의 잉크의 조합으로 색을 나타낸다. C(시안), M(마젠타), Y(노랑), K(검정) D있다.
2. ![image](https://user-images.githubusercontent.com/90343486/134359813-633c3b00-c054-4ddb-8408-89b4f379be3d.png)
#### HSV 색 공간
1. 색상(Hue), 명도(Value), 채도(Saturation) 기준이 되는 방식이다. 색상의 직관적이다. 시각 예술에 사용된다.
2. ![image](https://user-images.githubusercontent.com/90343486/134360090-a8a0ad0c-920b-492e-967a-e78c19a38d00.png)
3. 출저 https://ko.wikipedia.org/wiki/%EC%83%89_%EA%B3%B5%EA%B0%84


