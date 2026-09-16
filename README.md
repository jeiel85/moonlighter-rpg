# 🌙 Moonlight Merchant (문라이트 머천트)

> **주야간 듀얼 루프 던전 상점 경영 RPG (Single-File HTML5 Canvas & Web Audio API)**  
> 낮에는 상점에서 전리품을 팔아 최적 마진율을 탐색하고, 밤에는 고대 차원문 던전에서 희귀 유물을 파밍하여 30일 이내에 빚을 청산하는 듀얼 루프 RPG 타이쿤 게임입니다.  
> **🌐 한국어 / English 완전 다국어(i18n) 지원!**

---

## 🎮 게임 플레이 및 라이브 데모

- **웹 브라우저 즉시 플레이**: 별도의 설치나 빌드 과정 없이 `index.html` (또는 `moonlighter_rpg.html`)을 더블 클릭하거나 GitHub Pages 라이브 링크를 통해 플레이할 수 있습니다.
- **라이브 데모 링크**: [https://jeiel85.github.io/moonlighter-rpg/](https://jeiel85.github.io/moonlighter-rpg/)

---

## 🌟 핵심 시스템 특징

### 0. 🌐 완벽한 다국어 지원 (i18n Multi-Language)
- 상단 컨트롤 바의 **`🌐 한국어` / `🌐 English`** 버튼을 클릭하여 언제든지 즉시 언어를 전환할 수 있습니다.
- UI 텍스트뿐만 아니라 **25종의 아이템, 크래프팅 레시피, 손님들의 반응 대사, 몬스터 및 보스 명칭, 튜토리얼 도움말**까지 모두 한국어와 영어로 완벽히 지원됩니다.
- 선택된 언어는 `localStorage`에 자동 저장되어 새로고침 후에도 유지됩니다.

### 1. 낮: 상점 경영 시뮬레이션 (Day Shop Phase)
- **쇼케이스(Showcase) 진열 & 자율 가격 책정**:
  - 배낭 속 전리품을 원하는 가격(Gold)을 매겨 진열대에 등록합니다.
  - 진열대 슬롯은 상점 시설 투자를 통해 2칸에서 최대 8칸까지 확장할 수 있습니다.
- **손님 유형별 동적 가격 심리 AI**:
  - 🧑‍🌾 **마을 주민 (Villager)**: 기본 재료 선호, 가성비 중시
  - 🗡️ **모험가 (Adventurer)**: 무기/물약/방어구 선호, 실용적 가격 추구
  - 🧐 **수집가 (Collector)**: 유물/희귀 보석 선호, 높은 가격도 감수
  - 👑 **부유한 귀족 (Noble)**: 전설 유물 선호, 최고가 지불 용의
  - 🦹 **도둑 손님 (Thief)**: 방범 골렘이 없으면 물건을 훔치려 시도
- **이모티콘 반응 및 연속 판매 콤보**:
  - `🤑` (거저 주는 가격! 85% 이하 즉시 구매)
  - `😊` (적정 가격! 100~115% 만족 팁 지급 + 콤보 게이지 상승)
  - `🤔` (살짝 비쌈! 116~140% 확률적 구매)
  - `😡` (터무니없는 바가지! 구매 거부 후 분노 퇴장, 콤보 리셋)
  - 연속 적정가 판매 성공 시 COMBO 보너스로 최대 +50% 이상의 추가 마진 획득!

### 2. 밤: 2D 탑다운 액션 던전 크롤러 (Night Dungeon Phase)
- **부드러운 조작 & 액션 타격감**:
  - `W, A, S, D` / 방향키: 캐릭터 8방향 부드러운 이동
  - `마우스 좌클릭`: 근접 검 부채꼴 베기 (스윙 궤적 이펙트 + 몬스터 넉백 + 타격감)
  - `Q` 키 / `마우스 우클릭`: 원거리 활 사격 모드 전환 (화살 발사 투사체)
  - `Spacebar`: 무적 판정 구르기 회피 대시 (쿨다운 게이지 표시)
  - `E` 키: 보물상자 개봉 및 포탈 상호작용
- **4대 테마 절차적 던전 & 보스 인카운터**:
  1. 🌲 **숲 미궁 (Verdant Labyrinth)**: 슬라임, 독버섯, 덩굴 괴물 → **보스: 숲의 거신 (Forest Titan)**
  2. 🏜️ **사막 유적 (Sunken Ruins)**: 미이라, 모래 전갈, 유적 골렘 → **보스: 모래폭풍 파라오 (Dune Pharaoh)**
  3. 🌋 **용암 동굴 (Molten Cavern)**: 화염 임프, 불꽃 정령, 용암 게 → **보스: 용암 드래곤 (Lava Drake)**
  4. 🏛️ **고대 성소 (Ancient Sanctuary)**: 공허의 눈, 룬 수호병, 빛의 망령 → **보스: 차원 지배자 (Dimensional Overlord)**
- **16칸 배낭 인벤토리 관리**:
  - 25종의 다양한 전리품과 유물(Common, Uncommon, Rare, Epic, Legendary 등급)
  - 던전 안전 탈출 포탈 vs 심층부 보스 도전! (사망 시 소지품 일부 유실)

### 3. 마을 인프라, 대장간 & 크래프팅 (Town & Crafting)
- **대장간 (Blacksmith)**:
  - 검(공격력), 활(원거리 피해), 갑옷(최대 체력), 장화(이동속도) 단계별 제련 업그레이드
- **크래프팅 공방 (Crafting Bench)**:
  - 던전 전리품들을 조합하여 상점에서 큰돈을 벌 수 있는 고가 명품(비전 치유 물약, 숲의 수호궁, 태양신의 부적, 마그마 룬 소드, 차원 군주의 왕관 등) 제작
- **상점 인테리어 투자**:
  - 진열대 확장, 벨벳 카펫(이동속도/체류시간 증가), 방범 수호 골렘(도둑 방지), 수정 샹들리에(귀족/수집가 출현율 대폭 증가)

### 4. 30일 빚 청산 챌린지 (Debt Clearance 30-Day Challenge)
- 매 7일마다 찾아오는 상환 기한:
  - Day 7: 1,000 G
  - Day 14: 4,000 G
  - Day 21: 10,000 G
  - Day 28: 25,000 G
- 빚을 전액 청산하면 상점의 완전한 소유권을 획득하며, 무한 자유 모드로 영구 플레이 가능!

### 5. Web Audio API 신시사이저 & LocalStorage 자동 저장
- 외부 오디오 파일 없이 순수 브라우저 코드로 합성되는 타격음, 활 발사음, 계산대 카칭(Ka-ching!) 벨소리, 전리품 획득음 내장
- 골드, 인벤토리, 진열대, 장비, 날짜, 언어 설정 등이 `localStorage`에 실시간 100% 자동 보존됩니다.

---

## 🛠️ 기술 스택
- **Language**: HTML5, CSS3, Modern Vanilla JavaScript (ES6+)
- **i18n**: Built-in Bilingual Engine (Korean 🇰🇷 & English 🇺🇸)
- **Graphics**: HTML5 2D Canvas API (High-performance 60FPS Game Loop)
- **Audio**: Web Audio API (Procedural Sound Synthesizer)
- **Storage**: Browser LocalStorage API
- **Deployment**: GitHub Pages (Zero-dependency Single File Architecture)

---

## 📜 라이선스
MIT License
