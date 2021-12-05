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
5. 누크 같은것.  이미지를 지우면 알파채널로만 인식하고 지워진다.
### Straight Alpha
1. 특정 뷰어가 아닌 , 일반적인 뷰어로 보면 RGB가 알파에 매트화가 안되어있고, RGB색상과 alpha값을 그대로 받아 옵니다.
2. 반투명 상태의 값에서 원본에 없는 RGB 값이 보이거나 제거되어 보입니다. RGB색상 따로 알파 채널 따로 모두 따로 저장되어있습니다.
3. 매트 된 RGB + Alpha 채널이 꼭 있어야합니다.
4. RGB 채널은 그대로 유지되며 매트가 지정되지 않거나 지정된 색상으로 미리 곱해지지 않습니다.
5. 포토샵 . 같은것 사용자가 알파채널을 관리할 수없다. 투명한건 투명한거고 
6. ![image](https://user-images.githubusercontent.com/90343486/135484129-7a2da146-1117-4217-8bdc-c5e0132837e3.png)
7. 출처 https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=tjsdk666&logNo=120106782734, https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=micocu&logNo=220468841485
-----------------------------------------------------------
## 4Week
### Rotoscoping
> 애니메이션 기법 또는 VFX 기법의 하나다. 
> 촬영한 영상의 일부를 잘라내는 것이다. 움직이는 개체를 프레임별로 리드로잉 또는 마스킹하는 역할을 가진다.
1. 로토스코핑을 통해 불필요한 개체를 제거하거나 움직이는 요소를 동영상 푸티지에 추가할 수 있습니다
2. 생동감을 나타내고 합성할 때 여러 클립을 효율적으로 결합합니다.
3. 매트를 추출할 수 있는 도구
##### Rotoscoping 목적
1. 시퀀스의 특정을 정하고 영역을 추출한 다음에 마스크의 역할을 한다.
2. 이미지 시퀀스 작업할때 로토는 완벽해야 한다. 정확한 가장자리와 움직이는 물체와 그에 따른 모션 블러를 해서 분위기를 망치지 않아야한다.
3. 엣지로 정의 할 항목을 결정하고 전체 샷에서 원칙을 따라야한다,
4. 영상과 대상 물체의 모든 부분을 분석해야하며, 움직임의 요소에 따른 개체를 분할하는 위치를 정해야한다.
5. ![image](https://user-images.githubusercontent.com/90343486/136214402-61a0c5a6-44f7-42ba-b3b5-edb29e51d821.png)
6. 출처 https://namu.wiki/w/%EB%A1%9C%ED%86%A0%EC%8A%A4%EC%BD%94%ED%95%91 , https://www.leyong.blog/rotokeying/
## 5Week
### Keying (Chroma Keying)
> 두 개의 꽉 찬 프레임 영상을 합치는 비공식 용어로, 빛, 색의 값으로 정보를 구분해 낸다.
> 키잉은 요소를 더 빠르고 쉽게 분리 할 수있는 기술이다.
> 한 영상(A) 안에 다른 영상(B)과 겹처 색을 빼는 기술이다. 색상차이를 이용하여 피사체를 다른 화면에 합성하는 기법.
> 녹색과 청색이 피부나 머리카락의 색과 최대로 겹치지 않기때문에 자주 사용한다.
> 일관된 단색의 배경에서 특정 요소를 분리하는 프로세스이다.
##### 매트를 좀더 쉽게 뽑기 위한 방법,       알파를 좀더 쉽게 건드리는 방법
1. 키잉 작업을 하면 컴퓨터는 주어진 색상 범위를 정의하고 해당 픽셀을 제거한다.
2. 키잉은 컴 포지팅 응용 프로그램 내부에서뿐만 아니라 실시간으로 발생할 수도 있다.
3. ![image](https://user-images.githubusercontent.com/90343486/135488586-2e5eb3f8-ab2d-4638-b7ee-adcef4932a4a.png)
4. 출처 http://news.samsungdisplay.com/15102/ , https://www.leyong.blog/rotokeying/
### Checkerboard
> 검은색과 흰색 또는 적색과 검은색의 네모가 번갈아 격자로 배열된 모양이며, 체스 게임판의 체크 모양을 나타낸다.
> 체커보드 같은 패턴을 가진 물체를 이용하여 캘리브레이션의 정확도 및 효율성을 높일 수 있다.
1. ![image](https://user-images.githubusercontent.com/90343486/136217482-a2ca47b5-030c-434f-a110-66482f9c1784.png)
2. 출처 http://journal.ksae.org/xml/20100/20100.pdf
### Camera Calibration
> 우리가 실제 눈으로 보는 세상은 3차원이다. 하지만 카메라 상에서는 2차원의 이미지이다. 우리는 3차원 점들이 이미지 상에서 어디에 맺히는지 생각하면
> 영상 찍을 당시 카메라의 위치와 방향에 의해 결정된다. 실제 이미지는 렌즈와 이미지 거리 등 크게 영향을 받는다.
> 그래서 3차원 공간좌표 값, 피라미터값을 구하고 영향(이슈)받는걸 제거하는 과정을 카메라 캘리브레이션이라 한다.
1. 내부 피라미터 =  초점거리 , 주점 , 비대칭계수 가 있다.
2. ![image](https://user-images.githubusercontent.com/90343486/136217264-72a98286-8cae-44fc-b8cb-27fc0cddd455.png)
3. 출처 https://darkpgmr.tistory.com/32

### Merge
> Merge 노드는 다중 이미지를 레이어링 할때 쓰인다. 다양한 결합 연산(Merge Operation)으로 원하는 결과를 얻을 수 있다.
> A 와 B의 Input을 통해 데이터 연산을통해서 Output을 만든다.
> 매트합성과 블랜딩 합성이 주 분류로 이루며 RGB값에 의한 연산한다.
> 이미지 A를 B에다가 합성한다. A to B  대부분 배경을 이루는것이 B 그위에 올리는것이 A로 표현이 된다.
> 알파값이 중요하다. 곱셈 덧셈 나눗셈 뺄셈 같은것 수학적인 계산이 있다.
> Alpha가 있는 영역은 1, 없는 영역은 0
>  A- Input 된 이미지  a-  A의 알파값  
1. merge(plus) A+B 더하기
2. merge(minus) A-B 빼기
3. merge(multiply) AB 곱하기
4. merge(divide) A/B if A<0 and B<0 나누기
5. merge(average) (A+B)/2 A,B 두 이미지의 평균값. 결과는 원본보다 어두워진다. 
6. merge(over) A + B(1-a) 기본적으로 A가 premultiplied image.
7. merge(in) AB= B의 알파와 겹치는 이미지 A의 부분만 보여준다.
8. merge(mask) marge in 과 반대 개념.
9. merge(copy)A = A 연결된 이미지만 보여준다.
10. merge(from) A form b 이면 이미지 b에서 a를 뺀 영역만 보여준다.
11. merge(screen) A+B -AB
12. merge(under) A(1-b)+B = B의 알파값을 빼서 A와 곱한다음 B랑 더하는 값.
13. ![image](https://user-images.githubusercontent.com/90343486/136222159-4a293184-4de3-4e84-b454-3ec798900f52.png)
14. 출처 https://blog.naver.com/PostView.naver?blogId=s3dcomp&logNo=70134631359 , https://learn.foundry.com/nuke/13.0/content/comp_environment/merging/merge_operations.html
### Shuffle
> RGB 값과 Alpha 채널 등을 없애거나 생성시키거나 임의로 변경할 수 있는 기능.
### Invert
> 알파값 반전시키는 것.
## 6Week
### Keyers
키어는 다 독립적인 형태를 가진다.
1. 키라이트는 자동으로 스필제거를 해준다.
2. IBK keyer - IBK Gizmo, IBK Colour 2개의 노드가 있다. IBK Colour에서 수치를 조절하여 클린 플레이트를 만들 수 있다. IBK Gizmo 통해서 테크닉을 조절할 수 있다.
3. 출처 https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=loveandpic&logNo=221064084942
##### Utility
루미넌스채널 rgb채널 등을 조절할 수 있다.
##### Hue keyer
선택한 색(Hue)채널 뺄 수 있다
### Despill
> 그린스크린으로부터 넘쳐나는 Green 값을 제거해주는 연산
##### Difference
A, B 두 이미지 간의 매트로 입력이된다.
두 인풋의 알파 차이를 보는것 (포토샵 블랜딩모드랑 비슷함) 
## 7Week
### Tracking / Match move
> 카메라를 사용하여 시간이 지남에 따라 움직이는 물체를 찾는 과정, 변화를 추적합니다.
> 사용된 카메라의 3D시점, 줌, 내부 파라미터, 왜곡 등 카메라에 대한 모든 것을 복원 및 추적합니다.
1. ![image](https://user-images.githubusercontent.com/90343486/135489100-1d9facad-8834-4b5d-ad0f-5334531b58b3.png)
2. 출처 https://bskyvision.com/278 , https://darkpgmr.tistory.com/98
### NUKE tracking
>누크의 카메라 트래커는 카메라 추적을 통해 원래 카메라와 이동이 일치하게 가상 카메라를 만들 수 있습니다.
>Tracking 과 solve 를 통해 데이터를 추출해 낸다. 
>트레킹이 된 데이터에서 AutoTracks 창의 error max , max error 을 통해 불완전한 데이터를 정리해준다.
1. 1,2,3,4Points Tracking
2. 1point 중심이 되는 하나의 포인트를 선택하여 카메라의 위치값 움직임을 포착할 수 있다.
3. 2points 두개의 점을 통해 하나의 선을 통해서 카메라의 위치값 과 회전값을 포착할 수 있다.
4. 3points, 4points 3개, 4개의 점을 통해 면적을 만들고 카메라의 위치값, 회전값, 공간감(뎁스)를 포착할 수 있다.
### 3D Camera tracker
1. 하나의 가상의 공간에서 카메라를 생성하여 표현할 수 있다. 하나의 공간을 창조하여 카메라의 이동을 변경할 수있으며, 추가할 수 있다.
2. 공간을 만들어 내면서 focus length 뎁스, 위치값에 대한 키포인트를 나타내어 찾을 수 있다.
3. ![image](https://user-images.githubusercontent.com/90343486/139528627-1a342b45-d6cd-4584-b77a-b0635fe86b74.png)
## 9Week, 10Week, 11Week
### Visual Language
> 시각언어(Visual Languge)는 시각적 요소들을 이용한 소통 체계를 말한다.
> 한 개념을 각색하고 소통하게 하는 이미지로 시각 언어의 쓰임을 가정할 수 있다.
> 사람들의 생각을 '구두화'하는 것처럼, 시각 언어는 그것을 '시각화'할 수 있다.
1. 대상을 통해서 시각적인 인식을 하게 끔 하여 뜻과 표현을 상상할 수 있도록 하는것이다.
2. 출처 https://ko.wikipedia.org/wiki/%EC%8B%9C%EA%B0%81%EC%96%B8%EC%96%B4
#### pictogram
1. 그림문자이며 그림과 전달(telegram)의 합성어이며
2. 의미하고자 하는 바를 직접적으로 묘사한 그림을 통해 의미를 전달하는 표의문자이자 시각 디자인으로 사용된다.
3. ![image](https://user-images.githubusercontent.com/90343486/141686987-26d5fc96-ce42-48f4-96e7-df20e8b2f12a.png)
4. 출처 https://ko.wikipedia.org/wiki/%EA%B7%B8%EB%A6%BC%EB%AC%B8%EC%9E%90
### Contrast
> 대비와 비교를 나타낸다. 물체를 다른 물체와 배경과 구별할 수 있게 만들어주는 시각적인 특성의 차이
> 차이가 클수록 콘트라스트가 강하다
> 피사체를 돋보이게 할 수있고, 강한이미지, 딱딱한 느낌을 표현할 수 있다.
> 반면 너무 콘트라스트가 강하면 계조가 풍부하게 보이지 않는다.
1. 출처 https://ko.wikipedia.org/wiki/%EB%8C%80%EB%B9%84_(%EA%B7%B8%EB%A6%BC)
#### Value Contrast
1. 명도대비를 말한다.
2. 밝기가 다른 두 색이 서로 영향을 받아 밝은 색은 더 밝게, 어두운 색은 더 어둡게 보이는 현상.
3. ![image](https://user-images.githubusercontent.com/90343486/142588150-31a9f6a8-16ac-494a-bc70-7d29520a2907.png)
4. 출처 https://ys0317.tistory.com/63
#### Sharpness 
1. 선예도, 선명도를 말한다.
2. 선예도는 사진의 디테일이 얼마나 선명한지를 나타내며 질감을 강조하기 위한 가장 중요한 요소이다.
3. 카메라와 렌즈, 확대배율, 사진을 보는 거리 가 중요하다.
4. 첨예도(Acutance), 해상도(Resolution)과 관계가 있다.
5. ![image](https://user-images.githubusercontent.com/90343486/142589541-f14cf44c-1292-4424-babc-69527d706d02.png)
#### 첨예도(Acutance)
> 경계선에서 색이 얼마나 정확하고 순간적으로 변하는지 나타내는것.
> 첨예도가 높으면 경계선이 명확하다.
1. ![image](https://user-images.githubusercontent.com/90343486/142589452-9e2fc55f-4bee-4638-83c9-c65ca01ded56.png)
#### 해상도(Resolution)
> 근접한 선들을 구분해내는 카메라의 능력
> 해상도가 높으면 더욱 더 가는 선들을 구분할 수 있다.
> 얼마나 많은 것을 보여줄 수 있는가를 말한다. 디테일, 세밀하고, 자세하게 보여주는가?
1. ![image](https://user-images.githubusercontent.com/90343486/142589476-dae04829-eb5d-4522-8f65-c19102362179.png)
2. 출처 https://blog.daum.net/usstory/5264429, https://m.blog.naver.com/PostView.naver, isHttpsRedirect=true&blogId=velocity70&logNo=100019894586
#### Noise
> System을 방해하는 모든 전기 전자적인 요인을 말한다.
> 인위적 제어가 어려워 자연현상에서 나타나는 아주 작은 장해에도 민감하게 반응한다.
> 전기 전자기기에 전류가 유입되면, 이 전류 주위에 전계와 자계가 유도되고 또한 전위차에 의해 공간이 생긴 전계는 시간적으로 변화하면서 주위에 자계가 발생한다.
> 기기가 의도하는 바와 상관없이 전류가 흘러 불필요한 에너지인 전자파 노이즈가 발생한다.
1. ![image](https://user-images.githubusercontent.com/90343486/142590206-9cd0c76b-6061-4dfb-a7d1-bd75ca13a17b.png)
2. 출처 https://www.devicemart.co.kr/goods_process/get_html_to_string?url=/data/category/category_tech/00030005/00030005.html
### Aperture
>조리개를 뜻한다.
>눈의 동공과 같은 기능을한다. 빛이 통과하는 넓이를 조절하는 기능
>렌즈의 유효 직경을 변화시켜 주는 역할을 한다. 빛이 통과하는 ‘공간’을 가지고 빛의 양을 컨트롤하는 기능을 한다.
>F값이라 부른다. 
>조리개가 넓어지면 피사계 심도가 더 작아지며, 조리개가 좁아지면 피사계 심도가 더 커진다
>결과적으로 "초점이 맞는 범위"를 조절해준다.
1. ![image](https://user-images.githubusercontent.com/90343486/142590961-807dff2b-fb7e-417f-9abe-f380d0f28788.png)
2. 출처 https://blog.daum.net/sansu3160/172, https://tigerhelper.tistory.com/entry/%EC%B9%B4%EB%A9%94%EB%9D%BC-%EC%A1%B0%EB%A6%AC%EA%B0%9C%EA%B0%80-%EB%AD%94%EA%B0%80%EC%9A%94-%EC%A1%B0%EB%A6%AC%EA%B0%9C%EC%9D%98-%EC%97%AD%ED%95%A0%EC%9D%80
### Depth of field(DOF)
>피사계 심도를 말한다."초점이 맞는 거리"라고 할 수 있다.
>심도가 깊으면 원거리에서 근거리까지 초첨이 모두 선명한 상태로 촬영된다. (Pan Focus)
>심도가 얕으면 피사체의 일부분만 선명하게 촬영된다. (out of focus)
#### Depth of field 3요소
1. 조리개 값(f), 2. 초점거리, 3. 피사체와 거리
1. ![image](https://user-images.githubusercontent.com/90343486/142591666-0389689e-0c2c-42ff-89ba-4323f8118c30.png)
2. 출처 https://fantasy297.tistory.com/9 https://whiteknight3672.tistory.com/190 https://blog.daum.net/ayh12123/9148 https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=cinetaker&logNo=220264321194
## 10week, 11wwek, 12week
### Format Kinds
#### EXR FILE
>파일 EXR은 openEXR 비트 맵 파일이다. industrial light & magic 시각 효과 회사에서 만든 오픈 소스 hdr 형식 이미지 파일
>EXR 파일은 고품질 사진을 저장할 수 있으며, 무손실 또는 손실 압축으로 구성하여 여러 레이어를 지원하고 높은 휘도와 색상을 유지할 수 있다.
>다양한 사진 편집, 시각 효과 및 애니메이션 프로그램에서 사용된다.
>EXR 파일 포맷이란 HDR 이미지이다.
#### EXR 특징
1. 다른 픽셀 크기의 다중 채널을 지원한다.
2. 임의의 채널을 가질 수 있으며 왼쪽 및 오른쪽 카메라 이미지와 같은 여러 시점을 인코딩 할 수 있어 입체적인 기술을 지원한다.
3. HDRI 포맷
4. 오픈소스 라이센스로 로열티가 없다.
5. RGB 색상을 지원하고 무손실 압축을 한다.
6. Diffuse, Indirect, Beauty등 렌더 결과의 다양한 패스(A0V)의 이미지를 한 .exr 파일에 저장가능하다.
7. 각 픽셀에 추가적인 깊이(depth)정보를 여러개 저장하는 deep compositing을 통해 서로 복잡하게 교차하는 오브젝트들을 무리 없이 합성 가능하다.
8. HDRI, EXR 파일 추천 사이트 및 정보사이트 https://polyhaven.com/hdris
9. ![image](https://user-images.githubusercontent.com/90343486/144739218-13918d6f-0f2a-428b-83c2-6cad730d76a2.png)
10. 출처 https://ko.wikipedia.org/wiki/OpenEXR, https://ko.eyewated.com/exr-%ED%8C%8C%EC%9D%BC%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9E%85%EB%8B%88%EA%B9%8C/, https://namu.wiki/w/OpenEXR, https://www.lifewire.com/exr-file-2621157
#### HDR FILE (HDRI)
> (High Dynamic Range Image)
> 가장 밝은 곳부터 가장 어두운 곳까지, 눈으로 직접 보는 것과 최대한 가깝게 밝기의 범위를 확장하는 기술
> 서로 다른 사진을 합성하여 전체적으로 고르게 분포 된 색상 범위를 가진 단일 이미지를 만들 수 있다.
> 8bit 포멧 보다 수백배 많은 색상 정보를 가지고 있다.
1. 출처 https://ko.eyewated.com/hdr-%ED%8C%8C%EC%9D%BC%EC%9D%B4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9E%85%EB%8B%88%EA%B9%8C/, https://www.samsung.com/sec/tvs/tv-buying-guide/what-is-hdr-tv/, https://m.blog.naver.com/intenseardor/221736281026
#### DPX FILE
> 영화분야와 포스트프로덕션에서 DI(digital intermediate)작업과 영상효과(Visual Effects)작업을 위한 파일형식이다.
> 필름스캐너에서 스캔한 원래의 이미지에 대한 RAW이미지로 구성되어 있다.
> 각 채널에 대한 컬러농도를 표현하는 방식으로 잘 사용된다.
> 디지털이미지 처리 분야에 많이 사용된다.
> KODAK사의 cineon필름스캐너에서 사용되던 .cin파일을 개선하여 표준으로 정의된 파일형식이다.
> 비트맵
#### DPX 단점
1. 데이터용량이 크다.
3. 작업속도 면에서 영상시스템의 성능에 많이 치우쳐져있다. 성능이 안좋으면 시간이 많이 걸린다.
4. 출처 https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=hl1ixt&logNo=150118982264
### AOV
> (Arbitary Output Variables) 임의적으로 변경가능한 결과물이라는 뜻
> 사용자가 원하는 셰이딩 요소들을 따로 렌더할 수 있다.
> 렌더링 이후에도 이미지 조작및 수정이 가능하다.
> 그림자나 빛의 정보의 값을 얻을 수 있다.
> MAYA에서 AOV 기능을 통해 멀티패스 렌더링을 좀더 쉽게 할 수 있도록 해준다.
1. 출처 https://mogl3d.tistory.com/60, https://frauniemand.tistory.com/4
### Deep Compositing
#### Deep
> 딥 이미지 합성은 디지털 이미지를 합성 하고 렌더링하는데에 일반적인 색상 및 불투명도 채널 외에도 깊이 개념을 보여준다.
1. 단일 Z 깊이를 정의하지 않는 렌더링된 이미지의 데이터 채널을 제공하는 것을 목표로 한다. 
2. Z-깊이 이미지는 특히 투명도를 다루는데에 특화되어 있다.
3. 합성과 다른 형식의 데이터를 사용하여 디지털 이미지를 합성하는 방법이며, 추가 깊이 데이터를 사용한다.
4. 높은 이미지 품질이 생성되며 처리하기 까다로운 아티팩트의 문제들을 해결한다.
5. 2D 이미지를 가지고 깊이 있게 적절하게 합성할때 사용한다. 투명도, 블러, 자유도를 조절할 가능하며 자연스러운 합성 할 때 사용된다.
>  
>  ![image](https://user-images.githubusercontent.com/90343486/144740378-69e731f3-4d1c-4542-8595-6c4620632fb8.png)
>  ![image](https://user-images.githubusercontent.com/90343486/144740382-51766e8a-5ee6-46dd-9183-7f327322c856.png)
3. 출처 https://en.wikipedia.org/wiki/Deep_image_compositing, https://www.fxguide.com/fxfeatured/the-art-of-deep-compositing/, https://www.reddit.com/r/vfx/comments/1in6re/not_being_a_nuke_user_can_someone_explain_what/
### Scanline render & Raytracing render Difference
#### Scanline render
1. 렌더링된 이미지의 모든 픽셀을 통해 카메라의 광선을 전달한다.
2. 광선이 메쉬면을 가로지르는 경우 픽셀의 색상은 광원, 면의 선에 대한 각도, 해당 면에 대한 카메라의 각도 및 기타 정보에 따라 계산된다.
3. 매체가 없으면 픽셀은 배경색을 가져온다.
4. 렌더 속도가 매우 빠르다
5. 차지하는 메모리의 양이 작아 이슈가 작다.
6. 폴리곤과 함께 작동한다.
7. 반사, 투명도, 굴절의 표현이 어렵다.
8. 카메라에 보이는 물체를 제외하고는 모두 지워, 카메라 안에 위치한 물체만 뎁스 값에 따라 정렬한다.
#### Raytracing render
1. 장면의 광원을 분석하고 해당 조명에서 생성된 광선의 경로를 계산하여 컴퓨터가 최정 이미지를 생성하는 방식의 렌더러이다.
2. 결과는 반사 및 화선을 포함하며 매우 사실적인 이미지를 나타낸다.
3. 우리가 실제 세계에서 관찰한 것과 가까운 조명과 그림자이다.
4. 흡수, 반사, 투명도, 반투명도, 굴절 특성을 포함하여 픽셀의 최종 음영을 계산할 때 다양한 알고리즘을 고려할 수 있다. 편하다.
5. 렌더 속도가 매우 느리다
6. 차지하는 메모리양이 매우 많다.
7. 수학적 객체와 함께 작동한다.
8. 모든 지오메트리 정보를 담는다.
