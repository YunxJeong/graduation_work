# VR 재난 대응 교육 시스템
![Development Status](https://img.shields.io/badge/Status-In%20Development-green)
![Unity Version](https://img.shields.io/badge/Unity-2022.3.35f1-blue)
![C#](https://img.shields.io/badge/C%23-Latest-brightgreen)

> 감독관과 체험자 간 실시간 상호작용이 가능한 VR 기반 재난 대응 교육 시스템

## 목차
- [프로젝트 소개](#1-프로젝트-소개)
- [상세설계](#2-상세설계)
- [설치 및 사용방법](#3-설치-및-사용-방법)
- [소개 및 시연](#4-소개-및-시연-영상)
- [팀 소개](#5-팀-소개)

## 주요 기능
- 💻 실시간 모니터링 시스템
- 🎮 VR 기반 실감형 교육
- 🤝 감독관-체험자 실시간 상호작용
- 🎯 맞춤형 재난 상황 시뮬레이션

### 1. 프로젝트 소개
#### 1.1. 배경 및 필요성
 > 재난은 언제나 예측할 수 없고, 실제 상황에서 적절한 대처를 하는 것은 쉽지 않다. 이에 따라, 재난 발생 시 효과적으로 대응하는 능력을 길러주는 교육이 필수적이다. 특히 화재와 같은 긴급 상황에서의 대처 능력은 생명을 구하는 중요한 요소로 작용한다. 전통적인 교육 방식은 주로 이론적인 교육에 치우쳐 있어 실제 상황에 적응하는 데 한계가 있다. 이를 보완하기 위해 최근에는 가상현실(VR) 기술을 이용한 교육이 주목받고 있다.
 VR 기술은 사용자가 실제와 유사한 재난 상황을 체험할 수 있게 함으로써, 안전 대처 능력을 더욱 효과적으로 향상하는데 기여할 수 있다.

#### 1.2. 목표 및 주요 내용
 > 본 과제의 목표는 **체험자와 감독관 간의 실시간 상호작용**을 통해 맞춤형 재난 교육을 제공하는 데 있다. 주요 내용으로는 감독관이 체험자의 행동을 실시간으로 모니터링하고, 필요할 때 즉각적인 피드백을 제공함으로써, 기존 교육의 한계를 넘어서는 보다 **효과적인 재난 대응 교육**을 구현할 수 있다. 이러한 시스템은 체험자가 재난 상황에서 적절한 행동을 즉각적으로 습득할 수 있도록 도와줄 뿐만 아니라, **실질적인 대응 능력을 향상**시키는 데 기여할 것이다.


### 2. 상세설계
#### 2.1. 시스템 구성도
 ![시스템구성도1](https://github.com/user-attachments/assets/679f4759-5650-43d8-be30-ccc873808984)

> 시스템은 기본적으로 서버 역할을 하는 PC 감독관과 클라이언트 역할의 VR 체험자로 이루어져 있다.

 ![시스템구성도VR](https://github.com/user-attachments/assets/ff25a19f-4df9-44d4-b7ac-6acd5da58c82)
> 먼저 VR 체험자의 경우 VR 장비를 통해 접속한다. 이후 첫 UI를 통해 VR 체험자 버튼을 선택하게 되면 감독관의 IP를 입력하는 화면으로 넘어간다. 감독관으로부터 IP를 받아 붙여 놓은 후 시작버튼을 누르면 대기화면으로 들어감과 동시에 서버의 연결을 기다린다. 이후 감독관이 접속하여 서버를 생성하면 클라이언트로 접속하게 되고 감독관이 체험자의 환경 세팅을 끝내고 나면 VR 체험이 시작된다.

 
![시스템구성도PC](https://github.com/user-attachments/assets/dab159a3-b42f-42dc-a197-3eeb8eb7d6f8)
> PC 감독관의 경우는 개인 Laptop을 통해 접속한다. 이후 첫 UI에서 PC 감독관 버튼을 선택하게 되면 서버가 시작되고 체험자 환경 세팅 화면으로 진입한다. 세팅 화면에서는 체험자가 접속하면 세팅이 동작하며 세팅이 끝나고 시작 버튼을 누르면 VR 체험자도 체험을 시작하고, 실시간 모니터링을 시작한다.

#### 2.2. 사용 기술
<div align="center">
  <img src="https://img.shields.io/badge/Unity-000000?style=for-the-badge&logo=unity&logoColor=white"/>
  <img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white"/>
  <img src="https://img.shields.io/badge/Visual_Studio-5C2D91?style=for-the-badge&logo=visual%20studio&logoColor=white"/>
</div>

- 개발 도구: Unity 2022.3.35f1, Netcode for GameObjects 1.9.1, XRInteraction Toolkit 2.5.4
- 프로그래밍 언어: C#
- 버전 관리: Unity Version Control

### 3. 설치 및 사용 방법
1. 2개의 PC에서 각각 실행파일 폴더를 다운로드 받고 폴더 내의 "graduation project2.exe" 파일을 실행한다.

![시작화면](https://github.com/user-attachments/assets/1aa145e8-3cea-4cb7-a7c0-e27a6700453d) 
2. 시작 화면에서 한 PC에서는 PC감독관으로, 다른 PC에서는 VR체험자로 접속한다.

![ip입력](https://github.com/user-attachments/assets/6e5c48fe-6899-4aec-9ef4-aefba2167c37)
![ipconfig](https://github.com/user-attachments/assets/42c50b3d-0faa-40a2-b13c-ab7b25f5045f)
3. VR체험자의 경우 ip입력창으로 넘어간다. 여기서 PC감독관은 명령 프롬프트에서 ipconfig를 입력하여 IPv4 주소를 얻고 체험자에게 전달한다. 이후 감독관에게 받은 ip를 붙여 넣어주고 시작버튼을 눌러 대기화면으로 넘어간다.

![세팅화면](https://github.com/user-attachments/assets/dc3fc507-4f95-4a74-bd28-00bc865986bc)
4. 감독관은 접속 후 세팅화면에서 플레이어 세팅을 하고 시작을 누르면 VR체험자의 화면이 바뀌며 시뮬레이션을 시작한다.


### 4. 소개 및 시연 영상
#### 4.1 소개
1. VR체험자 화면
![vr화면](https://github.com/user-attachments/assets/8ace2257-ec58-4916-94ab-0f1351a37365)
> VR 체험자는 감독관이 세팅한 상황들을 바탕으로 재난상황을 체험할 수 있다.

2. PC감독관 화면
![pc화면](https://github.com/user-attachments/assets/a015ba07-936e-41d6-bb7a-df77db5749b6)
> PC감독관은 미니맵과 화면을 통해 VR체험자를 모니터링할 수 있으며, 주어진 버튼을 통해 상호작용이 가능하다.

#### 4.2 시연 영상
[![2024년 전기 졸업과제 13 모션일이고](http://img.youtube.com/vi/iOX_i1il5Sw/0.jpg)](https://www.youtube.com/watch?v=iOX_i1il5Sw&list=PLFUP9jG-TDp-CVdTbHvql-WoADl4gNkKj&index=13)    


### 5. 팀 소개
  * 이종민
    * Email: jomgminlee@gmail.com
    * 기기 간 네트워크 연결 및 세팅(Netcode)
    * 1:1 의사소통 기법 구현(미니맵, 마커)
    * UI 디자인 및 최적화
    * 음성 채팅 구현(Vivox)
  * 노윤정
    * Email: roghkcool@gmail.com
    * VR 작동 환경 구현
    * 가상환경 속 상호작용 구현
    * 가상환경 수정 및 보완(벽, 바닥, 계단 등)
  * 장승우
    * Email: tmddn531@naver.com
    * 시나리오 구성
    * ui구성 및 동작
    * 네트워크 보조 (체험자 따라가는 카메라)
    * 환경세팅(체험자 위치이동, 물건 배치)
