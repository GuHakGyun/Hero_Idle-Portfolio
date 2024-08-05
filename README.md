# Hero_Idle-Portfolio
# 1. 게임소개
<div align="center">
    <img src="https://github.com/user-attachments/assets/8f1f233b-a746-44b0-b84c-eaac6eaeff3d" alt="pngScreenShot" style="display: block;">
    <span style="display: block; margin: 0; padding: 0; line-height: 0;"><게임 이미지></span>
    </div><br/>

* 유니티를 배우면서 팀프로젝트를 통해 제작한 2D 방치형 게 포트폴리오 입니다.
* 개발기간 : 2024. 04.22 ~ 2024.05.17 ( 약 4주 )
* 형상관리 : Git SourceTree
<br/>

# 2. 개발 환경
* Unity 2022.3.25f1 LTS
* C#
* Window 10
<br/>

# 3. 참여인원 및 역할

| 참여 인원 | 역할 |
| ------------ | -------------------------------- |
| 구학균(본인) | 플레이어 애니메이션 구현, 스킬 이펙트 및 효과음 구현 |
| [김양현](https://github.com/yangstar98) | 몬스터 스폰, 몬스터 효과음 구현, 로고 제작, 배경음 구현|
| [김재훈](https://github.com/JaerHoon) | 스탯 설정, 인벤토리 UI구|
<br/>

# 4. 사용 기술 
| 사용 기술 | 설명 |
| ------------ | -------------------------------- |
| 디자인 패턴| 싱글톤을 활용하여 Manager 관리 <br> ScriptableObject를 이용하여 플레이어 기본 능력치 설정 |
| 유한상태머신| 파라미터에 따른 애니메이션 연출 |
| Layer Mask| Layer를 활용하여 플레이어가 범위 내 몬스터를 인식함 <br> 자동사냥 버튼 클릭 시 인식한 몬스터를 자동으로 추적 및 공격**|
| Json| 게임 종료시 Josn 데이터로 저장하여 관리 |
| Object Pooling| 자주 사용하는 객체는 Pool로 관리(몬스터,투사체,코 등) |
<br/>

# 5. 구현 기능
- Object
    - 플레이어
        - 전사
        - 궁수
    - 일반 몬스터
         - 해골전사 2종(일반전사, 강화전사 - 피격시 캐릭터 밀어냄)
         - 해골법사(마법 투사체 공격)
         - 해골궁수(화살 공격)
    - 보스 몬스터
        - 골렘 => 기본공격,투사체 발사 및 낙석떨구기 스킬 시전
    - NPC
        - 로비에 NPC가 있으며 버튼을 눌러 상호작용
        - 아이템 획득 오브젝트
    - 아이템
        - 패시브 아이템 7개(상태이상 및 능력치 증가)
        - 공격 아이템 3개
- 스킬
    - 전사
        - 기본공격(근접) + 기본공격 강화 3종류
        - 스킬 + 스킬 강화 3종류
        - 방어스킬 - 방패이용
    - 궁수
        - 화살공격(원거리) + 공격 강화 3종류
        - 스킬 + 스킬 강화 3종류
        - 방어스킬 - 보호막 생성
- 스테이지
    - 로비
    - 전투 맵
    - 아이템 상점
    - 보스 맵
- UI
    - Scene
      - TitleScene : 게임로고, 시작버튼
      - CharacterChoice : 캐릭터 정보 확인, 버튼을 눌러 캐릭터 선택
      - Main Scene : 로비,스테이지,캐릭터 및 몬스터 HP,코인 획득,스킬 쿨타임 확인등
                     게임 진행을 위한 Scence
    - Popup
        - NPC 대화창,옵션창
        - 스킬설명 - 스킬 및 아이템 UI에 마우스를 갖다대면 스킬설명창 생성
<br/>

# 6. 개발 일지
<br/>

# 7. 플레이 영상

