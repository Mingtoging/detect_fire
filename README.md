본 프로젝트는 대전 인력개발원의 [ROS 기반 자율주행 드론 개발자 과정]을 통하여 수료한 프로젝트 입니다.


# 프로젝트 이름 : 화재탐지 드론
# 프로젝트 수행 기간 : 2021. 07. 01 ~ 09. 08

사용 기술 요약 : Open_CV와 머신러닝(cascade)을 활용한 객체 감지 기술 입니다.

project 요약 설명 : 화재 신고를 받은 드론이 화재지점으로 날아가 순찰 모드를 활성화 시키고 화재를 탐지시 경고 알람과 문자(좌표)를 사용자에게 보내줍니다.
                   사진은 실시간 으로 켑쳐되어 컴퓨터에 저장 되고 초기진화 시도를 위한 소화탄을 낙하 후 복귀합니다.

개발환경 : Ubuntu 18.04 , R.O.S_melodic

HW : bebop Parrot

시뮬레이션 환경 : Gazebo

팀원 :  이선환, 이주현, 조민석, 한정훈

자세한 내용은 안의 보고서와 youtube를 참고해주세요.

YouTube -- > "https://www.youtube.com/channel/UCLSgng38L1zVYUgOHEe1yOg/videos"

# 사용 알고리즘
<div align = "center">
  
![ff](https://user-images.githubusercontent.com/84003327/131608391-6c4307f9-928f-4680-8425-be5165bc3eac.png)
  
 </div>
 
드론은 목표지점으로의 이동을 위한 G.P.S코드가 있습니다. 위성을 통해 제공받은 G.P.S 정보를 바탕으로 드론이 이동하여야 하는 지점을 특정할 수 있습니다. 저희 팀에서는 많은 실험을 통하여 이동간 오차 범위와 속도 등의 최적의 컨트롤 값을 얻을 수 있었습니다. 

또한 드론이 탐색, 정렬간 북쪽을 바라보도록 설정하였는데 이를 통해 드론의 위치도 지도상의 정확한 사방위를 쉽게 파악할 수 있게 되었습니다.

또한 cv_bridge를 사용 하여 R.O.S환경에서 Open_CV를 사용할 수 있게 만들었으며, 코드에cascade Data를접목시켜 화재인식의 대한 성능을 향상 시켰습니다.


# 결과 화면
![img_fire](https://user-images.githubusercontent.com/84003327/131607360-730ae13d-a02d-4515-8e73-5fca24717e04.png)

![m4](https://user-images.githubusercontent.com/84003327/131608551-e0af671f-dca0-4183-b1b2-aa9ae668827e.png)



