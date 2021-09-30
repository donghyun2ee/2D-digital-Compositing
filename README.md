첫 기터부. 등록
# 2D-Digital-Compositing
## 2Week
### 2D
-------------------
2D의 정의 평소의 우리가 아는 2d란 X, Y축으로 보여지는 그래픽의 요소 하지만 그것은 수학의 정리 이다.  2D 디지털에 관련된 것은 결과 매체가 2D 라는것.
> 디지털 어희
1. Bit: 데이터의 단위 0이나 1의 값을 가진다. 배타적인 상태이다. ex).모스부호 
2. Digit: 0~9 까지의 아라비아 숫자
3. Vector: 표현 vector2 (x,y) vector3 (x,y,z) vector4 (x,y,z,w)
4. Integer: 소숫점이 필요없다. 0,1,2,3,4...
5. Float: 0.1, 2.35, 3.142...
6. Boolean: 0(off) or 1(on)  ex 레이어를 껏다 켰다. - 불린데이터 
### Compositing
> Compositing(합성)
1. 둘 이상의 것을 합쳐서 하나를 이룬다.
### Color
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
### Alpha
알파란 무엇인가.
> Alpha 채널 
> 알파 채널 또는 알파 합성은 a채널과 이미지 처리 분야에 있고, 각 화소에 대해 색상 표현의 데이터로 보조 데이터를 말한다.
1. Alpha 값은 0.0(완전 투명색) ~ 1.0(완전 불투명) 으로 표현이이 된다.
2. ![image](https://user-images.githubusercontent.com/90343486/134357688-8289b809-ce68-4a40-8c71-52b25d59ed53.png)
3. 출처 https://ko.wikipedia.org/wiki/%EC%95%8C%ED%8C%8C_%EC%B1%84%EB%84%90
### Color space
Color space(색공간) 무엇인가.
> 색공간은 색 표시계(color system)를 3차원으로 표현한 공간의 개념이다. 모든 색들은 이 색 공간에서 3차원 좌표로 나타낸다.
### 색 표시계
1. 색 표시계는 CIERGB, CIEXYZ, CIELAB, CIELUV 등의 색 체계를 말한다.
2. 디자인 학계나 산업계에서 색채 디자인 또는 시각 디자인등 카메라, 스캐너, 모니터, 프린터 등에 사용
3. 컬러 영상 장비 개발 및 응용 단계에서 색 공간은 정확한 색 표현을하기위해 필수적이다.
4. 디지털, 디자인에서 사용되는 색 공간은 CIELAB 색공간이며, 먼셀 색 표시계의 기본 원리 색의 3속성(색상(hue), 명도(Value), 채도(Saturation)를 사용한다.
### RGB 색 공간
1. 색을 혼합하면 명도가 올라가는 가산 혼합 방식이다. R(레드), G(그린), B(블루) 의 삼원색이 있다.
2. ![image](https://user-images.githubusercontent.com/90343486/134359532-9262ac8b-5205-4dc0-8055-4d747c21ffac.png)
### CMYK 색 공간
1. 색을 혼합하면 명도가 낮아지는 감산 혼합 방식이다. 인쇄과정에서 쓰이며, 네 가지의 잉크의 조합으로 색을 나타낸다. C(시안), M(마젠타), Y(노랑), K(검정) D있다.
2. ![image](https://user-images.githubusercontent.com/90343486/134359813-633c3b00-c054-4ddb-8408-89b4f379be3d.png)
### HSV 색 공간
1. 색상(Hue), 명도(Value), 채도(Saturation) 기준이 되는 방식이다. 색상의 직관적이다. 시각 예술에 사용된다.
2. ![image](https://user-images.githubusercontent.com/90343486/134360090-a8a0ad0c-920b-492e-967a-e78c19a38d00.png)
3. 출처 https://ko.wikipedia.org/wiki/%EC%83%89_%EA%B3%B5%EA%B0%84
-----------------------------------------------------------------------
## 3Week
### Gamma
> 감마는 디스플레이에 입력되는 신호의 밝기, 화면상에 나타나는 영상 휘도(디스플레이 기기의 밝은 정도) 간 관계를 결정하는 수치이다.
> 감마의 역할은 컴퓨터 화면 상에서 디지털 이미지가 어떻게 보이는지에 크게 영향을 준다..
> 밸런스를 맞춰주는 기능이며 이미지의 정확한 색과 밝기를 표현한다.
> 쉽게 말해 눈이 색깔의 변화를 느끼는 정도의 차이가 다르기 때문에 디스플레이의 색상의 단계를 정한 것이다.
> 적합한 이미지 품질을 얻기 위해 인체 시야의 비선형성을 보상하는 밝기 값 인코딩을 나타낸다.
1. 이유: 사람의 눈은 컬로보다 밝기 차이에 민감하다. 세포는 밝기에 반응하는 세포수가 컬러반응 세포보다 절대적으로 많다.
2. 사람의 눈은 베버의 법칙 때문에 밝은 색보다 어두운 색에 훨씬 민감하다.
### 감마의 세가지 유형
1. 이미지 감마 - 카메라 또는 RAW 이미지 변환 소프트웨어에서 JPG, TIFF 같은 압축 파일로 변환할때 사용한다.
2. 디스플레이 감마 - 컴퓨터, 모니터, 비디오 카드 등에서 이미지 출력을 조정할때 사용된다. 높은 디스플레이 일수록 감마는 더 어둡고 대비가 있는 이미지를 만든다.
3. 시스템 감마 - 이미지를 표시하는 데 사용되는 모든 감마 값을 나타낸다. 본질적으로 이미지와 디스플레이 감마를 결합한 것이다.
### 감마값
1. 각 채널에 주어진 전압에 대한 휘도와의 관계가 비선형으로 주어지는데 이러한 비선형 관계가 감마이다.
2.  감마가 1일 경우 입력, 출력 값이 동일
3.  감마가 높으면 입, 출력 값 증가
4.  감마가 낮으면 입력 대비 출력 값의 변화가 느리다.
5.  ![image](https://user-images.githubusercontent.com/90343486/135304286-8a3db363-0789-4eae-bfca-2951de6bc734.png)
6.  CRT(음극으로 부터 방출된 전자의 흐름 선관) 감마 곡선 + 카메라 감마 보정 = 최종시청상태
7. ![image](https://user-images.githubusercontent.com/90343486/135307314-043e48aa-633c-45f7-99e1-1fd3db71ee52.png)
8. 출처 https://blog.daum.net/trts1004/12109543 , https://ko.eyewated.com/%EA%B0%90%EB%A7%88-%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B4%EB%A9%B0-%EC%82%AC%EC%A7%84%EC%97%90%EC%84%9C-%EC%96%B4%EB%96%BB%EA%B2%8C-%EC%82%AC%EC%9A%A9%EB%90%A9%EB%8B%88%EA%B9%8C/ , https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=happynano&logNo=220433057440
### CRT
> CRT = Cathode-Ray Tube의 약자. 브라운관 방식의 디스플레이 장치이다.
1. ![image](https://user-images.githubusercontent.com/90343486/135309425-d7159b27-98b2-4219-b942-76cc27d1645b.png)
2. 그림처럼 전자총에서 전자를 발사하여 화면에 발려진 형광물질과 충돌하여 빛을 낸다.
3. 전자총에선 RGB의 3가지 색이 나오고 전자석을 사용하여 원하는 위치로 전자를 보낸다.
4. 원하는 위치와 원하는 강도로 빛을 보내 화면상에 나온다.
### CRT 모니터 장점과 단점
##### 장점
1. 반응속도 빠르다.
2. 색재현률이 좋다.
3. 저해상도에서 픽셀이 크게 보이거나 심하게 뭉게지지 않는다.
4. 색상왜곡이 적고, 색상이 화사하다.
##### 단점
1. 부피가 크고 무겁다.
2. 전기를 많이먹는다.
3. 수명이 짧다. 전자총의 출력과 형광물질의 양이 달라 주기적으로 캘리브래이션 해주어야 한다
4. 눈위 십게 피로해진다.
5.  출처 https://lucycle.tistory.com/44
### Linear Workflow
> 실제 세상의 빛은 Linear로 작용한다. 빛의 양은 광원들의 빛의 양을 합친 값이며 실제 세상에서는 input(전압 공급)이 output(이미지 환산)과 일정하다. 그것을 linear 이다.
> Linear Workflow(선형 워크플로우)는 모든 그래픽 작업이 선형 색 공간(Linear Color Space)에서 이루어지는 방식을 말한다.
1. jppeg 같은 이미지 파일들은 이미 감마 보정을 통해 발게 만들어진 이미지이다. 이런 이미지들을 임의로 수정, 효과를 적용하면 왜곡된 결과가 나온다
2. 선형 색 공간에서 작업하는게 권장 되며,이를 리니어 워크플로우라고 한다.
3. 리니어 워크플로우에서 작업된 이미지는 마지막 랜더시 다시 감마 보정을 통해 밝게 만들어지고, 렌더된 이미지는 디스플레이 장치에서 다시 어둡게 조정되어 우리가 보고자 하는 이미지로 출력된다.
4. ![image](https://user-images.githubusercontent.com/90343486/135314272-c32148d1-152c-4857-8368-2adb93932e19.png)
5. ![image](https://user-images.githubusercontent.com/90343486/135314310-ba9f5fd2-a7a4-4fd0-9774-e0604b74626f.png)
6. 출처 https://frauniemand.tistory.com/8 , https://kyoungwhankim.github.io/ko/blog/color_linearworkflow/
### ACES (AP0)
> Academy Color Encoding System으로 불려지며, 시스템은 색상을 관리하기 위한 업계의 차세대 표준 기술이다. 
> 디지털 영상을 만드는 카메라는 다양한 종류만큼 다양한 색역 계조범위를 가지고있는데 그것을 통합된 색공간 안에서 할 수 있도록하는 기술이다.
##### 장점
1. 색보정 불확실성을 줄인다
2. 넓은 색공간의 색심도를 가진다. 
3. 자유로운 창작 환경을 제공한다.
4. 인간이 볼 수 없는 공간까지 고려한 색공간이있다.
### ACEScg
> ACES의 색공간을 말한다. 
> 인간의 가시영역을 나타내는 CIE XYZ 1931 과
> 디지털 시네마 환경 영역을 나타내는 sRGB(일반 모니터), Rec.709(HDTV 포맷) Rec.2020(UHDTV 포맷), DCI-P3(극장용 프로젝터), 등의 색공간을 포함한다.
> CIE 도표는 인간이 볼 수 있는 모든 색 영역을 나타낸다.
1. ![image](https://user-images.githubusercontent.com/90343486/135316594-9bf4d2a2-7a40-4ade-8d3b-8a32821690c3.png)
2. ACEScg 색 영역은 디지털 구현된 모든 색 공간을 커버한다. 어떤 카메라로 찍든간에 ACES 색상 표준에 넣기만 하면 모든 팀이 같은 색 환경에서 작업이 가능하여 편하다.
3. 출처 https://m.blog.naver.com/loveandpic/221221809613 , https://artnfear.com/entry/ACES-%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%9D%B4%EB%9E%80
### Premultiplied Alpha
1. Premultiplied는 RGB 값이 이미 합쳐저 파일에 저장 되기 때문에 일반 뷰어로 원본이미지와 같은 이미지로 볼 수 있습니다.
2.  채널 구성에는 매트 된 RGB + AlPHA 채널이 없어도 문제가 없습니다. RGB로 바로 보아도 알파가 적용된 이미지 형태입니다.
3. 컴포지스트 플에서 배경 색을 설정하여, 블랙이나, 화이트를 설정가능하고 배경과의 문제를 해결할 수 있다.
4. 매트 방식으로 처리되어 모든 처리 방식이 가시화되어 저장됩니다.
### Straight Alpha
1. 특정 뷰어가 아닌 , 일반적인 뷰어로 보면 RGB가 알파에 매트화가 안되어있고, RGB색상과 alpha값을 그대로 받아 옵니다.
2. 반투명 상태의 값에서 원본에 없는 RGB 값이 보이거나 제거되어 보입니다. RGB색상 따로 알파 채널 따로 모두 따로 저장되어있습니다.
3. 매트 된 RGB + Alpha 채널이 꼭 있어야합니다.
4. RGB 채널은 그대로 유지되며 매트가 지정되지 않거나 지정된 색상으로 미리 곱해지지 않습니다.
5. ![image](https://user-images.githubusercontent.com/90343486/135484129-7a2da146-1117-4217-8bdc-c5e0132837e3.png)
6. 출처 https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=tjsdk666&logNo=120106782734, https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=micocu&logNo=220468841485
### Rotoscoping
> 애니메이션 기법 또는 VFX 기법의 하나다. 
> 촬영한 영상의 일부를 잘라내는 것이다.
1. 로토스코핑을 통해 불필요한 개체를 제거하거나 움직이는 요소를 동영상 푸티지에 추가할 수 있습니다
2. 생동감을 나타내고 합성할 때 여러 클립을 효율적으로 결합합니다.
3. 출처 https://namu.wiki/w/%EB%A1%9C%ED%86%A0%EC%8A%A4%EC%BD%94%ED%95%91
