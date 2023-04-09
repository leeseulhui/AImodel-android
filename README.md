# AImodel-android
opensource / Project to implement artificial intelligence model on Android phones

지난번 '나의 손글씨로 숫자 인식하기 프로젝트' 와 연결하여 이번에는 안드로이드 폰에서 AI 모델로 손글씨를 써서 숫자를 얼마나 정확하게 인식하는지 해보았다.
** 지난번 프로젝트 링크 : https://github.com/leeseulhui/MyHandwriting

Android studio를 사용하였다. Device Manager를 등록하여 가상 장치를 등록해주었다.

![image](https://user-images.githubusercontent.com/75656859/230780930-7c713bf7-a5bd-4adb-b6f5-6b2e99a71f5d.png)

그리고 MainActivity에서 만든 가상 장치를 실행시킨다.

![image](https://user-images.githubusercontent.com/75656859/230781033-003f829a-8b6d-4381-aa03-5b5aa9b9402f.png)

여기서 나는 "Manifest merger failed" 라는 첫 번째 오류가 발생하였다.
정확히는 
![image](https://user-images.githubusercontent.com/75656859/230781129-70cb79c4-39e0-4f4f-8b02-572a47dbd02d.png)
이런 오류이다. 오류가 나서 해결책을 찾아보니 Android 12를 타겟팅하는 경우 AndroidManifest.xml 파일에서 adroid:exported를 true로 설정해주어야 한다고 한다. 
따라서 추가해주었다.
![image](https://user-images.githubusercontent.com/75656859/230781205-0e334420-76ca-4af5-a890-64bb6eec1a32.png)

그랬더니 잘 작동되었다.

실행결과이다.

![image](https://user-images.githubusercontent.com/75656859/230781233-489c7e54-9c37-482c-b3cb-3052f14c9109.png)
![image](https://user-images.githubusercontent.com/75656859/230781245-db354d11-207e-4fac-add3-22a4656b3cca.png)

정확하게 예측하고 있는 것을 볼 수 있다.


