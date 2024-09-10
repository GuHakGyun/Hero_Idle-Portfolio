# Hero_Idle-Portfolio
# 1. 게임소개
<div align="center">
    <img src="https://github.com/user-attachments/assets/8f1f233b-a746-44b0-b84c-eaac6eaeff3d" alt="pngScreenShot" style="display: block;">
    <span style="display: block; margin: 0; padding: 0; line-height: 0;"><게임 이미지></span>
    </div><br/>

* 유니티를 배우면서 팀프로젝트를 통해 제작한 2D 방치형 게임 포트폴리오 입니다.
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
| Layer Mask| Layer를 활용하여 플레이어가 범위 내 몬스터를 인식함 <br> 자동사냥 구현 => 버튼 클릭 시 인식한 몬스터를 자동으로 추적 및 공격|
| Json| 게임 종료시 Josn 데이터로 저장하여 관리 |
| Object Pooling| 자주 사용하는 객체는 Pool로 관리(몬스터,투사체,코인 등) |
<br/>

# 5. 구현 기능
- Object
    - 플레이어
        - 전사
    - 일반 몬스터
        - 슬라임
        - 거미
        - 박쥐
        - 드래곤
    - 아이템
        - 무기,방어구 및 장신구
        - 코인(능력치 강화)
        - 보석(장비뽑기)
- 스킬
    - 액티브 스킬
        - 어스퀘이크
        - 토네이도
        - 칼날바람
        - 메테오
    - 버프 스킬
        - 플레이어 능력치 강화 스킬   
- UI
    - Scene
      - TitleScene : 게임 로고 및 시작버튼, 배경연출(구름 움직임)
      - LoadingScene : 시작버튼 클릭 시 로딩화면 구현, 배경 및 LoadingBar 제작
      - MainScene : 플레이어 및 몬스터, 조이스틱, HP, 데미지, 스킬슬롯 및 UI, 자동공격 버튼, 가이드퀘스트창 등 </br> 게임플레이에 활용되는 Scene
    - Popup
        - 캐릭터 정보창, 장비창, 스킬창, 퀘스트창, 장비뽑기창, 인벤토리창,옵션창
        - UI내 버튼 클릭시 해당 창이 Popup
<br/>


# 6. 플레이 영상
[유튜브](https://youtu.be/t9l6iQSmiPc)
