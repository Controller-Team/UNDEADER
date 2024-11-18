<div align="center">
<img src="./Source/Image/GameLogo.png" width="633" height="126" />
<br>
<br>
<h2>[2024 졸업 프로젝트] 🎮 UNDEADER</h2>
수수께끼의 좀비 바이러스로 인해 멸망해버린 세계.<br>
더 이상 군대는 힘을 잃었고, 남은 생존자들 마저 죽음을 두려워해 바깥으로 나가지 않는다.<br>
희망의 빛이 꺼져가던 그 때, 결코 죽지 않는 불사의 힘을 가진 존재가 총 두 자루를 들고 나타나는데...<br>
</div>



## 개요
![GameBanner](https://github.com/user-attachments/assets/f008395f-2864-4613-aff9-954e536af559)

- 프로젝트 이름: Undeader
- 프로젝트 기간: 2024.03 ~ 2024.11
- 개발 엔진 및 언어: Unreal 5.2, BluePrint
- 멤버: 팀 컨트롤러(박준형, 한 강, 최희선, 한혜원)
- 장르: 3D 탑뷰 슈팅액션 로그라이크

## 핵심 기술

- BluePrint로 플레이어, 몬스터, NPC 등의 다양한 객체 설계 및 실시간 액션에 따른 상태 변화 구현
- 애니메이션 리타게팅, 몽타주, 에임 오프셋 등 FPS에서 필요한 ABP 구현
- PlayFab GBaaS 게임 클라우드 서버 글로벌 랭킹, 데이터 저장 및 불러오기

## 게임 설명
|![타이틀스샷](https://github.com/user-attachments/assets/8fd56da2-b0cc-4e8b-85db-6879e4df20f9)|![언데더스샷](https://github.com/user-attachments/assets/a8a21353-9908-46e6-9e4e-fa3282875413)|
|:---:|:---:|
|게임 타이틀|게임 플레이 화면|

- ⚔️ **몰려드는 좀비와 전투**<br>
이 세계에는 다양한 좀비들이 등장하는 구역이 존재합니다.<br>
좀비들을 지닌 총으로 모두 토벌하고, 다음 구역으로 넘어가십시오.
- 🏃‍♂️ **다양한 총기류와 악세사리 액션**<br>
스태미나를 관리하고, 회피를 사용해 위협으로부터 달아나십시오.<br>
더 등급이 좋은 피스톨과 라이플, 악세사리를 장비하고 좀비들을 격퇴하십시오.
- 🆙 **NPC 구출과 업그레이드**<br>
곳곳에 숨겨진 NPC들을 구출하고, 앞으로의 게임에서 영구적인 업그레이드를 받으세요.<br>
보상과 상점에서 나오는 기어를 통해 더 좋은 아이템을 지급받고 시작합니다.
- 💀 **세 종류의 구역과 보스**<br>
총 세 종류의 구역에서 다양한 상호작용이 가능합니다.<br>
스테이지의 끝에 도달하고, 보스와 전투해 승리하십시오.
- 🏆 **랭킹 서버와 클라우드** <br>
게임을 시작하면, 계정을 만드십시오. 글로벌 랭킹에 당신의 플레이타임이 랭크됩니다.<br>
또한, 어디서 게임을 즐기던 클라우드 저장과 불러오기를 통해 데이터를 유지하십시오.<br>

## 게임 플레이 방식
- 캐릭터 이동 방법

| 이동방향 | 상(위) | 좌(왼쪽) | 하(아래) | 우(오른쪽) | 사격 | 회피 | 장전 | 달리기 | 상호작용 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 키보드 | W | A | S | D | 마우스 좌클릭 | SPACE | R | SHIFT | F |
| 게임패드 | ⬆️ | ⬅️ | ⬇️ | ➡️ | RT | LT | X | B | A |

- 구역

|좀비 구역|상점 구역|휴식 구역|
|---|---|---|
|![좀비구역 스크린샷](https://github.com/user-attachments/assets/d37d430b-7be8-4a95-9269-7cc6930a3bad)|![상점구역 스크린샷](https://github.com/user-attachments/assets/0a07a2fd-b3dc-43cf-b480-f6491ed36670)|![휴식구역 스크린샷](https://github.com/user-attachments/assets/5ca88d29-f4d3-456e-9718-83465756d330)|
|난이도가 다른 좀비들과의 전투|무기 구매 및 판매|HP 재충전 및 휴식, 시간 정지|

- 스테이지

## Youtube 소개 영상

[![Video Label](http://img.youtube.com/vi/s06XNfH2WD4/0.jpg)](https://youtu.be/s06XNfH2WD4)
[![Video Label](http://img.youtube.com/vi/M4robE6cgFE/0.jpg)](https://youtu.be/M4robE6cgFE)
- 위 섬네일을 클릭 시 유튜브로 이동합니다.

## 세부 기술 소개

![image](https://github.com/user-attachments/assets/3940fe58-c52d-40a1-906b-f550e0964929)

### 게임 클라이언트: Unreal Engine 5.2

- **게임 플레이 요소**
  - 플레이어의 **HP**, **스태미나**, **돈** 등 상태 표시.
  - 제한 시간 내 **좀비 처치 및 생존** 목표.
  - **라이플**과 **피스톨** 두 종류의 무기 사용.
  - 최대 **8개의 악세사리** 획득 및 장착 가능.
  - 좀비 처치 시 **경험치**와 **돈** 획득.
  - 레벨업으로 **공격력/치명타/체력/돈 획득량 강화**.
  - 생존 시 **무기/악세사리/돈/기어** 등의 보상 제공.
  - 두 갈림길 중 하나를 선택해 다음 던전 입장.

- **3D 애니메이션 및 액션**
  - 플레이어와 좀비 캐릭터를 파츠(머리, 몸통, 팔 등) 단위로 본 애니메이션 적용.
  - **팩토리 메서드 패턴**으로 수십 개 총기를 모듈화.
  - **무적 회피 기동**, **볼트 액션** 등 액션 요소 구현.

- **게임 시스템**
  - **게임 상태 직렬화**를 통해 바이너리 파일로 저장/복원 가능.
  - **Behavior Tree**와 **EQS**를 활용한 NPC의 동적 의사 결정(경로 찾기 및 상호작용).

- **그래픽 및 인터페이스**
  - 절차적 던전 생성으로 매번 다른 플레이 경험 제공.
  - **포스트 프로세싱**으로 그래픽 품질 향상 및 가려진 오브젝트 처리.
  - HUD의 변수와 로직 변수를 분리, **클라이언트 보안 강화**.
  - 입력 매핑으로 **키보드/마우스/조이스틱** 등 통합 관리.
  - **게임 옵션** 메뉴로 일시 정지 및 볼륨 조절 기능 제공.

---

### 게임 서버: Azure Playfab

- **데이터 관리**
  - 유저의 게임 데이터를 **클라우드에 저장 및 동기화**.
  - 클라이언트 데이터와 서버 데이터를 대조해 **무결성 검사 및 비동기 로드**.

- **리더보드 시스템**
  - 전 세계 유저 데이터를 관리하고 **주간 초기화** 로직 적용.
  - 유저 정보 및 국기를 클라이언트에 표시.

- **보안 강화**
  - 유저 로그인 이력 로깅으로 보안성 강화.


## 개발자들

| 이름 | Git Username |
| --- | --- |
| 박준형 | <a href="https://github.com/suldangoo"><img src="https://img.shields.io/badge/suldangoo-181717?style=flat-square&logo=GitHub&logoColor=white" height="28px"/></a> |
| 한 강 | <a href="https://github.com/kangtoe"><img src="https://img.shields.io/badge/kangtoe-181717?style=flat-square&logo=GitHub&logoColor=white" height="28px"/></a> |
| 최희선 | <a href="https://github.com/heesunc"><img src="https://img.shields.io/badge/heesunc-181717?style=flat-square&logo=GitHub&logoColor=white" height="28px"/></a> |
| 한혜원 | <a href="https://github.com/Hye-won-Han"><img src="https://img.shields.io/badge/HyewonHan-181717?style=flat-square&logo=GitHub&logoColor=white" height="28px"/></a> |
