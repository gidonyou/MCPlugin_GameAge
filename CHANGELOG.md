# 패치 내역
모든 패치 기록은 여기에 첨부 될것입니다. 버전마다 도움을 주실경우 패치에 추가해 드립니다.

## 1.0.0 - 2018-1-22
*방송후 버그/밸런스 패치 -- 최종 패치*

**도움을 주신분:**

베타 테스터: NF3charcoaL, J\_arvi\_S, TF2\_ValS

### 게임 시작
  - 도움을 주신 분 리스트가 업데이트 되었습니다.
  - 게임 설정은 OP 에게만 알려줍니다 (설정에서 사용 안할수 있음). 
  - 아이템 배분 시스템 다시 코딩  
> 상자 갯수가 많을경우 실패 횟수가 많아지면  
> 서버가 튕깁니다. 방지하기 위해 추가:  
> 서버 설정: `MAX_CHEST_TRIAL`
  - 도움을 주신분: 베타 테스트를 도와주신 분들 추가.
  - '문법 오류 수정 작업을 도와주셨습니다.' 으로 변경.
> 아 그리고 제 이름 뜰 때  
> 문법 오류 수정 작업을 도와주셨습니다. 뭐 이런  
> 까리한 말 좀 써주시지요  
> 맞춤법을 모르는 저를 도와주셨습니다 볼 때마다  
> 눈물 나옵니다

### 설정
  - config.yml 을 추가해서 플러그인 설정이 쉬워집니다.
  - /play 명령어로 서버 설정 업데이트가 가능해집니다. (아래 명령어 확인)
  - 설정 추가: `BROADCAST_CONFIG`
    - 설명: 게임 시작시 설정을 OP 에게 알려줍니다.
    - 방법: 0 - 알려주지 않음  |  1 - 알려줌
    - 기본값: 0 - 알려주지 않음
  - 설정 추가: `MAX_CHEST_TRIAL`
    - 설명: 상자 설치할때 몇번까지 시도할지 정합니다
    - 방법: W : 0 ~
    - 기본값: 1000000  (상자 1000개 까진 되는듯 하네요)

### 명령어 
/game 명령어 
  - OP 이상 사용가능하도록 설정.

/play 명령어
  -  g, r, i, b, f - OP 전용 명령어로 변경.
  - 추가: /play s - 설정을 보여줍니다.
  - 추가: /play rl - config.yml 을 다시 불러옵니다. (오피전용)
  - 추가: /play u - 설정 목록을 알려줍니다. (오피전용)
  - 추가: /play u \[설정이름] - 설정 현재 값을 알려줍니다. (오피전용)
  - 추가: /play u \[설정이름] \[정의] - 설정을 업데이트 합니다 (오피전용)

### 아이템 패치

#### LOCATION_FINDER (나침판) 
  - 드롭 : 25 → 5 (10.96% → 3.94%)
    
#### PLAYER_TIME_ABOVE (많은시간)
  - 드롭 : 15 → 11 (6.58% → 8.66%)
  
#### PLAYER_TIME_ABOVE (적은시간)
  - 드롭 : 15 → 11 (6.58% → 8.66%)
  
#### PLAYER_TIME_LIST (시간 목록)
  - 드롭 : 10 → 6 (4.39% → 4.58%)
  
#### DIAMOND_SWORD
  - 드롭 : 3 → 3 (1.32% → 2.36%)
  
#### IRON_SWORD
  - 드롭 : 12 → 16 (5.26% → 12.21%)
  
#### STONE_SWORD
  - 드롭 : 20 → 20 (8.77% → 15.27%)
  
#### SHIELD
  - 드롭 : 18 → 0 (7.89% → 0%)
> 재미가 없다는 의견으로 다음 업데이트에서 없어질 예정

#### FIRST_AID
  - 드롭 : 20 → 20 (8.77% → 15.27%)
  - 치유 : 5칸 → 4칸
  - 쿨타임 추가: 6초
  
#### BANDAGE
  - 드롭 : 35 → 30 (15.35% → 22.90%)
  - 치유 : 2칸 → 1.5 칸
  - 쿨타임 추가: 3초
  
#### STEAL_TARGET
  - 드롭 : 15 → 2 (6.58% → 1.53%)
  
#### EARN_SECONDS
  - 드롭 : 40 → 7 (17.54% → 5.34%)
  
#### 총합
  - 드롭 228 → 131
  
### 버그패치
  - 게임이 2+ 이상 시작될시 강제 경기구역 데미지가 쿨타임 없이 즉시 시작되는것 패치. (테스트 안해봄)  


## [Beta 3 RC] - 2018-1-20
*방송 테스트때 썻던 버전*

### 추가
- 도움을 주신 분 목록 15초 추가

### 수정

#### 패치
나침판 소리 패치

#### 임시수정
스폰서 메세지 제거

#### 아이템 드롭
- 다이아 칼 : 5 --> 3
- 철 칼 : 10 --> 12
> 다이아 칼 드랍률이랑
> 철칼 드랍률이 딱 두 배 차이나네요
> 다이아 3개에 철 12개 이렇게 해두는 게 더 낫지 않을까요  (- 목탄님)

#### 맞춤법
*목탄님 추천*

  - 방패 아래
    - 설명 수정: "자신을 방어할 때 이용합니다." 
  - 나침판
    - 설명 수정: "자신보다 많은 시간을 가지고 있는 사람의 위치를 알려줍니다."
  - 적은 시간 유저
    - 설명 수정: "자신보다 적은 시간을 가지고 있는 사람의 위치를 알려줍니다."
  - 붕대
    - 설명 수정: "자신의 체력을 최대 2칸까지 치유합니다."
  - 구급상자
    - 설명 수정: "자신의 체력을 최대 5칸까지 치유합니다."
  - 상대방 수명 뺏기
    - 설명 수정: "지목 상대에서 시간을 뺏습니다."
  
  
### 위키 수정
*보통 위키는 업데이트 로그를 안남기지만 이번것은 남깁니다.*
위키 수정 (맞춤법 수정한것과 동일)

  - 죽음의 책
    - 위키: 사진 수정 (위키)
  - 나침판
    - 이름 수정: "가리키는 나침판" (위키)
  - 기본칼
    - 설명 수정: "게임이 시작될 때." (위키)
  - 돌 칼
    - 설명 수정: "한 단계 업그레이드되었습니다." (위키)
  - 다이아 칼
    - 설명 수정: "무기 중 가장 높은 데미지를 가지고 있습니다." (위키)

## [Beta 2 RC] - 2018-1-17
### 추가
- README.md 에 위키 정보 추가.

## [Beta 1 RC] - 2018-1-17
개발 완료... 컨텐츠 진행후 릴리스 대기중.