# Ancestor's Map — DD Field Guide

**[⬇ Download / 다운로드 / ダウンロード / 下载](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest)**

> Developed with AI assistance (Claude, Codex) — design, in-game testing and final decisions by the author.<br>
> AI(Claude · Codex)의 도움으로 개발했습니다 — 기획 · 게임 확인 · 최종 판단은 제작자가 직접 합니다.<br>
> AI（Claude・Codex）の支援を受けて開発しました。企画・ゲームでの確認・最終判断は作者自身が行っています。<br>
> 本工具在 AI（Claude、Codex）的协助下开发——策划、游戏内测试与最终决定均由作者亲自完成。

<details>
<summary><img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1f0-1f1f7.png" width="20" alt="🇰🇷"> <b>한국어 설명서</b></summary>

다키스트 던전 1의 **지도 · 전투 정보 · 활동 일지**를 게임 위에 띄워 주는 오버레이입니다.

항상 최상위 창으로 떠서 전체화면 게임 위에 겹쳐지고, 앱을 클릭해도 입력은 게임이 그대로 받습니다. **게임 화면 위에 겹쳐 두고 쓰는 것을 권장합니다.**

바닐라 정보를 고정으로 넣어 둔 것이 아닙니다. **지금 불러온 세이브에 켜진 본편 + DLC + 모드 데이터를 적용 순서대로 읽어 병합**하므로, 모드가 추가하거나 바꾼 골동품 · 적 · 장신구 · 기벽도 실제 인게임 값 그대로 보입니다. 이름과 설명은 게임 번역을 사용하며, 다른 세이브를 불러오면 알아서 다시 맞춥니다. 도감 검색란에 글을 쓸 때는 앱이 입력을 받습니다.

<p align="center">
<img src="images/anim_battle.ko.webp" width="49%" alt="고른 전투 기술에 따라 대상별 피해와 효과 수치가 바뀌는 모습">
<img src="images/anim_map.ko.webp" width="49%" alt="지도 칸에 마우스를 올리면 카드가 뜬다">
</p>

### 무엇이 되나

- **전투 화면** — 고른 기술의 피해·명중·치명타·효과 확률을 대상 위에 표시합니다. 아군 지원, 자리 이동, 적이 고른 기술과 대상, 현재 상태와 다음 차례의 지속 효과도 볼 수 있습니다.
- **탐험 중 선택** — 골동품·장애물·허기짐 카드에서 결과를 보고 선택지를 누릅니다. 함정 카드에서는 영웅별 해체 확률과 스트레스를 비교한 뒤 해체할 영웅을 고릅니다.
- **함정 앞 자동 멈춤·소지품 정리** — 정찰된 함정 앞에서 멈추고, 가방 단추나 `[I]`로 소지품을 정리합니다. 가방에 마우스를 올리면 게임의 소지품·전리품 칸에 판매가를 표시합니다.
- **상세 지도** — 골동품 결과, 적 구성, 남은 칸, 필요한 보급품, 목표까지의 길과 정찰·밝기 보정을 확인합니다.
- **기록과 마을 준비** — 활동 일지·미터기·영웅 표, 도감 검색, 추천 보급품(던전 추가 모드 포함)과 자동 구매, 건물·추가 건물 요구 재화 계산을 제공합니다.
- **화면 안내** — 물음표 단추에서 7장 31단계 안내를 엽니다. 녹화된 견본 장면을 보며 따라가고, 일부 단계에서는 직접 마우스를 올려 카드를 볼 수 있습니다.

### 화면

<table>
<tr><td align="center" width="50%"><img src="images/card_curio.ko.webp" alt="맨손과 열쇠의 결과를 비교하고 선택할 수 있는 골동품 카드"><br><sub>골동품 카드</sub></td><td align="center" width="50%"><img src="images/card_trap.ko.webp" alt="영웅별 함정 해체 확률과 스트레스"><br><sub>함정 해체</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/heroes.ko.webp" alt="마을 영웅 표와 장비·기술 카드"><br><sub>영웅 표와 카드</sub></td><td align="center" width="50%"><img src="images/supplies.ko.webp" alt="던전과 원정 길이별 보급품 추천 표"><br><sub>보급품 추천</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/meter.ko.webp" alt="영웅별 원정 수치를 비교하는 미터기"><br><sub>원정 미터기</sub></td><td align="center" width="50%"><img src="images/codex.ko.webp" alt="도감 검색과 적 카드"><br><sub>도감</sub></td></tr>
</table>

### 자세히

<details>
<summary>기능별 설명 펼치기</summary>

#### 전투

- 전투가 시작되면 기본 화면의 지도가 전투 화면으로 바뀝니다. 아군 차례에는 고른 기술이 닿는 대상들의 수치를, 적 차례에는 적이 선택한 대상의 수치를 표시합니다. 회복·강화·이동 기술도 해당 배치로 보여 줍니다.
- 인물 위 두 열에서 걸린 상태와 남은 기간, 다음 차례의 지속 효과량을 구분합니다. 지속 피해로 체력이 소진될 것으로 예상되면 핏자국으로 알립니다. 아래에는 체력과 스트레스가 표시됩니다.
- 아래 초상에 마우스를 올리면 영웅·적의 전투 카드가 뜹니다. 현재 장비·기벽·질병·강화와 조건을 반영한 수치, 적의 기술·대상 선택 확률을 비교할 수 있습니다. 스킨과 변신·태세도 현재 모습에 맞춥니다.
- 턴 순서, 스톨링의 증원 위험, 후퇴 확률을 표시합니다. 턴 순서·후퇴 결과는 기본으로 켜져 있으며 가운데 타이틀을 눌러 끌 수 있습니다. 끄면 후퇴는 확률만 보입니다. 타이틀에 마우스를 올리면 원정 미터기가 뜹니다.

#### 지도와 탐험

- 방·복도·골동품·함정·장애물·전투·허기짐 칸을 표시합니다. 기본은 밝혀진 구역만 보기이며, 안개를 끄면 전체를 볼 수 있습니다. 목표 골동품·보스·안뜰의 경로는 열쇠와 잠긴 문의 순서를 고려합니다.
- 아래 계수기에서 남은 칸을, 보급품 그림에서 그 품목의 사용처를 확인합니다. 전투·허기짐 아이콘으로 아직 가 보지 않은 칸의 적 구성과 허기짐 칸 표시를 따로 끌 수 있습니다. 정찰 확률, 밝기 보정, 특수 조우의 위치 또는 출현 조건도 볼 수 있습니다.
- 게임에서 골동품·장애물·허기짐 창이 열리면 대응하는 카드가 뜹니다. 열을 누르면 게임의 선택지를 실행하며, 골동품 아이템 열은 해당 아이템을 사용합니다. 보급품이 부족한 열은 실행하지 않습니다.
- 정찰된 함정 앞 자동 멈춤은 기본으로 켜져 있으며 함정 계수기로 끕니다. 해체는 자동으로 하지 않습니다. 카드에서 영웅을 고르면 그 영웅으로 해체를 시도합니다.
- 탐험 대기 중 가방 단추나 `[I]`로 같은 품목 묶음을 합치고 칸을 정리합니다. 퀘스트 아이템은 제자리에, 빈 칸은 뒤에 둡니다. 전투 후에는 전리품 창을 닫고 탐험으로 돌아왔을 때 기본 원정대로 자동 복귀합니다. 기본으로 켜져 있으며 원정대 단추로 끕니다.

#### 기록과 마을 준비

- 활동 일지는 전투·탐험·야영 기록을 계속 쌓으며 `[End]`로 엽니다. 전투가 시작돼도 일지로 자동 전환하지 않습니다. 세이브별 최근 원정 10개와 종결 미터기를 다시 볼 수 있습니다.
- 마을 영웅 표에서 레벨·원정·걸음과 앱이 기록한 누적 수치를 비교합니다. 초상에 마우스를 올리면 장비·전투 기술·야영 기술이 보입니다.
- 보급품 표는 던전·원정 길이에 맞는 추천 수량을 보여 줍니다. 켜 둔 던전 모드(안뜰+, 농장+, 태양을 향한 섬들, 버민타이드, 악마의 축제)의 던전도 함께 나오고, 고른 퀘스트의 줄을 강조해 그 던전을 표 맨 위로 올립니다. 줄을 누르면 구매·되팔기·비용 미리보기, **6초 안에 같은 줄을 다시 누르면 실행**합니다. 범위는 큰 값으로 맞추고 무료 지급품은 되팔지 않습니다. 핏빛 저주 영웅을 위한 피도 조절하며 마을에 남는 쇠약 영웅 몫을 남깁니다.
- 도감에서 적·장신구·마을 이벤트·질병·각성·붕괴·기벽을 이름·등급·직업·효과로 검색합니다. 건물·추가 건물 화면에서는 고른 증축에 필요한 재화와 보유량을 비교합니다. 계획 기능이며 게임에서 대신 건설하지 않습니다.

</details>

### 설치

1. [최신 릴리스](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest)에서 `AncestorsMap.zip`을 받아 아무 폴더에 풉니다.
2. `AncestorsMap.exe`를 실행합니다. **.NET 8 Desktop Runtime**이 없으면 설치 안내가 뜹니다.
3. 게임을 실행하면 세이브를 자동으로 찾습니다. 처음에는 오른쪽 위 물음표 단추로 화면 안내를 열어 보세요.

### 요구·호환

- Windows 10/11, [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0), 설치된 Darkest Dungeon 1이 필요합니다. 앱 실행 파일은 약 **5.7MB**이며 런타임은 별도입니다.
- 실시간 정보와 입력 보조는 지원하는 **64비트** 게임에서 사용합니다. 스팀 공개판·`coming_in_hot` 베타의 스팀 및 DRM 없는(`_windowsnosteam`) 실행 파일을 지원합니다. 32비트·인식하지 못하는 게임 버전에서는 메모리를 읽지 않고 세이브 기반 기능만 제공하며, 일지 상태 줄에 이유를 표시합니다.
- 활성 DLC·모드와 적용 순서를 읽어 반영합니다. 던전 추가 모드는 Courtyard Plus, Farmstead Plus, The Sunward Isles, Vermintide, The Fiend Festival로 확인했습니다. 모든 모드를 검증한 것은 아닙니다.
- 스팀 설치를 기준으로 하며 DRM 없는 실행 파일도 확인했습니다. GOG 등 다른 플랫폼은 설치·세이브 경로를 자동으로 찾지 못할 수 있습니다.
- 한국어·English·日本語·简体中文을 지원합니다. 처음에는 게임 언어를 따르고, 이후에는 앱에서 선택한 언어를 사용합니다.

### 안전

- **게임 파일·세이브·게임 메모리에 직접 쓰지 않으며, 게임 프로세스에 코드를 주입하지 않습니다.** 메모리는 읽기 권한으로 엽니다. 앱 자체의 설정과 원정 기록은 따로 저장합니다.
- **입력 보조 기능은 실제 게임 조작입니다.** 방 이동, 카드 선택과 아이템 사용, 함정 해체, 자동 구매, 소지품 정리, 기본 원정대 설정은 게임에 클릭·키·끌어 놓기 입력을 보냅니다. 이 조작의 결과는 게임의 정상 저장에 반영될 수 있습니다.
- 함정 앞 자동 멈춤은 이동 키·마우스 버튼을 떼는 입력과 이동 키 반복 차단을 사용합니다. **기본 켬**이며 함정 계수기로 끕니다. 전투 후 자동 원정대 복귀도 **기본 켬**이며 원정대 단추로 끕니다.
- 가방에 마우스를 올려 판매가를 볼 때도, 탐험 중 게임이 지도 탭이면 `[Tab]` 입력으로 소지품 탭을 엽니다. 보기 기능 중에도 이처럼 입력을 보내는 경우가 있습니다.
- 자동 구매·정리 중에는 마우스를 움직이지 마세요. 정리할 때 `[Shift]`를 누르지 마세요. 게임의 버리기 조작과 겹쳐 앱이 끌어 놓기를 진행하지 않습니다.
- 앱의 통신은 GitHub 릴리스 확인입니다. 시작할 때 자동 확인하며 앱 정보에서 수동으로 다시 확인할 수 있습니다. 계정·API 키가 필요 없고 게임 기록을 업로드하지 않습니다.
- 다른 프로그램의 메모리를 읽어 일부 백신이 오탐할 수 있습니다. 다운로드 검증에는 릴리스에 제공된 SHA-256을 사용하세요.

### 업데이트

새 버전이 있으면 시작할 때 알려 줍니다. 왼쪽 위 서명을 클릭하면 현재 버전과 **업데이트 확인**을 볼 수 있습니다. 새 버전 안내에서 릴리스 페이지를 열고 새 zip을 받으세요. 자동 다운로드·교체는 하지 않습니다. 실행 중인 앱을 종료하고 새 파일을 덮어쓰면 됩니다. 설정과 원정 기록은 `%LocalAppData%\AncestorsMap`에 남습니다.

### 조작

| 키·마우스 | 동작 |
|---|---|
| <code>[`]</code> 또는 화면 숨기기 단추 | 촛불 단추만 남기기. 촛불 클릭 또는 같은 키로 복귀 |
| `[Backspace]` | 기본 화면으로: 마을 영웅 표 / 보급품 표 / 탐험 지도 / 전투 화면 |
| `[Home]` / `[End]` | 도감 / 활동 일지 열기·닫기 |
| `[Caps Lock]` | 지금 기본 원정대 설정 |
| `[I]` 또는 가방 클릭 | 탐험 대기 중 소지품 정리 |
| 가방에 마우스 올리기 | 게임 소지품·열린 전리품 칸의 판매가 |
| 원정대 그림 클릭 | 전투 후 기본 원정대 자동 복귀 켜기·끄기 |
| 왼쪽 끌기 / 오른쪽 끌기 | 앱 창 이동 / 지도 이동 |
| 휠 / 휠 클릭 | 지도 확대·축소 / 안개 켜기·끄기 |
| 앱 지도의 이어진 방 클릭 | 방 안에 있을 때 게임에서 그 방으로 이동 |
| 자동으로 뜬 카드의 열 클릭 | 골동품·장애물·허기짐 선택 또는 영웅을 골라 함정 해체 |
| 보급품 줄 클릭 → 6초 안에 같은 줄 클릭 | 구매 미리보기 → 자동 구매 |
| 창 경계 끌기 / 위 슬라이더 | 창 크기 / 배경 불투명도 |
| 물음표 / 서명에 마우스 올리기·클릭 | 화면 안내 / 조작표·앱 정보 |

게임 위 단축키는 게임 창이 앞에 있을 때 동작합니다. `[I]`는 탐험 대기 중에만 앱이 가져가며, 그 밖에는 게임의 원래 키로 동작합니다. 앱 자체에서는 <code>[`]</code>·`[Home]`·`[End]`도 사용할 수 있고, 검색란에 글이 있을 때 `[Backspace]`는 글자를 지웁니다. 구매·정리는 게임 창을 활성화하며, 방 이동·카드 선택·함정 해체 등도 게임 창이 앞에 있어야 합니다.

### 화면 안내

물음표 단추에서 처음 사용, 지도, 탐험 중 선택, 전투, 원정 관리, 마을 준비, 기록과 검색을 살펴보세요. 처음 6장은 녹화된 견본 장면이므로 게임을 실행하지 않아도 볼 수 있습니다. 마지막 ‘기록과 검색’ 장은 사용자 자료를 엽니다. 마우스를 올릴 수 있는 단계에서는 금색 테두리 안에 올려 보세요. 어두운 곳을 누르거나 앱을 숨기면 안내를 닫습니다.

### 알려진 한계

- 적 구성·허기짐 칸·턴 순서·후퇴 결과 등 게임이 숨기는 정보도 표시합니다. 필요한 항목만 켜서 사용하세요.
- 게임이 업데이트되면 지원 여부를 확인할 때까지 실시간 기능을 사용할 수 없습니다. 일부 세이브 기반 표시는 게임이 저장할 때까지 늦을 수 있습니다.
- 추천 보급품은 위키·공략·던전 생성 규칙을 참고한 값이며, 모드 던전은 계산 추정치를 포함합니다. 원정대와 탐험 계획에 맞춰 조절하세요.
- 자동 입력은 게임 화면과 배치에 영향을 받습니다. 지원하지 않는 배치나 일부 모드에서는 기능이 제한될 수 있습니다.

### 문제 신고

[Issues](https://github.com/Eolaloe/DD-AncestorsMap/issues)에 앱 버전(서명 클릭), 게임 버전(공개판 / `coming_in_hot` / DRM 없는 판), 활성 모드 목록, 어느 화면에서 어떤 조작을 했는지 적어 주세요. 가능하면 스크린샷과 앱에 나온 알림 문구도 첨부해 주세요.

### 라이선스 · 크레딧

[LICENSE](LICENSE) — 개인 사용 자유, 공유는 공식 저장소 링크로(파일 재업로드 · 수정본은 문의), 판매 금지.
Darkest Dungeon 은 Red Hook Studios 의 게임입니다.
Claude · Codex 의 도움을 받아 만들었습니다.

</details>

<details>
<summary><img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1ef-1f1f5.png" width="20" alt="🇯🇵"> <b>日本語の説明</b></summary>

Darkest Dungeon 1の**マップ・戦闘情報・アクティビティ・ログ**をゲーム画面に重ねて表示するアプリです。

フルスクリーンのゲームの上にも常に最前面で重なり、アプリをクリックしても入力はそのままゲーム側に届きます。**ゲーム画面の上に重ねて使うことをおすすめします。**

バニラの情報を固定で埋め込んでいるわけではありません。**いまロードしているセーブで有効な本編・DLC・MODのデータを適用順に読み込んで統合する**ので、MODで追加・変更されたキュリオ・敵・トリンケット・奇癖も、実際のゲーム内の数値どおりに表示されます。名前や説明にはゲームの翻訳を使い、別のセーブをロードしても自動で合わせ直します。図鑑の検索欄に文字を入力するときはアプリ側に切り替わります。

<p align="center">
<img src="images/anim_battle.ja.webp" width="49%" alt="選んだスキルに応じて対象ごとのダメージや効果の数値が変わる戦闘画面">
<img src="images/anim_map.ja.webp" width="49%" alt="マスにマウスを乗せるとカードを表示">
</p>

### できること

- **戦闘画面** — 選んだスキルのダメージ・命中・クリティカル・効果の確率を対象の上に表示します。味方への支援、移動、敵が選んだスキルと対象、現在の状態と次のターンの継続効果も確認できます。
- **探索中の選択** — キュリオ・障害物・空腹のカードで結果を確認し、そのまま選択肢を実行できます。トラップカードでは英雄ごとの解除確率とストレスを比べ、解除する英雄を選べます。
- **トラップ手前での自動停止・所持品整理** — 偵察済みのトラップの手前で停止します。バッグのボタンか[I]で所持品を整理でき、バッグにマウスを合わせるとゲームの所持品・戦利品の枠に売却額を表示します。
- **詳細マップ** — キュリオの結果、敵の編成、残りのマス、必要な補給品、目標への経路、偵察確率や明るさの補正を確認できます。
- **記録と村での準備** — ログ・メーター・英雄表、図鑑検索、おすすめ補給品（ダンジョン追加MODを含む）と自動購入、建物・区画に必要な資源の計算を利用できます。
- **画面ガイド** — はてなマークから全7章・31ステップの案内を開けます。録画した見本の場面で説明し、一部のステップではマウスを合わせてカードを見ることもできます。

### 画面例

<table>
<tr><td align="center" width="50%"><img src="images/card_curio.ja.webp" alt="素手と鍵の結果を比べて選べるキュリオカード"><br><sub>キュリオカード</sub></td><td align="center" width="50%"><img src="images/card_trap.ja.webp" alt="英雄ごとのトラップ解除確率とストレス"><br><sub>トラップ解除</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/heroes.ja.webp" alt="村の英雄表と装備・スキルのカード"><br><sub>英雄表とカード</sub></td><td align="center" width="50%"><img src="images/supplies.ja.webp" alt="ダンジョンと遠征の長さ別のおすすめ補給品"><br><sub>おすすめ補給品</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/meter.ja.webp" alt="英雄ごとの遠征成績を比べるメーター"><br><sub>遠征メーター</sub></td><td align="center" width="50%"><img src="images/codex.ja.webp" alt="図鑑の検索と敵のカード"><br><sub>図鑑</sub></td></tr>
</table>

### 詳しい機能

<details>
<summary>機能ごとの説明を開く</summary>

#### 戦闘

- 戦闘が始まると、基本画面がマップから戦闘画面に切り替わります。味方のターンでは選んだスキルが届く対象の数値を、敵のターンでは敵が選んだ対象の数値を表示します。回復・強化・移動スキルも、それぞれに合った配置で表示します。
- キャラクターの上の2列には、付与中の状態と残り期間、次のターンの継続効果量を分けて表示します。継続ダメージでHPが尽きる見込みなら血しぶきで示します。下には現在のHPとストレスを表示します。
- 下段の肖像にマウスを合わせると戦闘カードが開きます。現在の装備・奇癖・病気・強化や条件を反映した数値と、敵のスキル・対象選択確率を比べられます。スキン、変身、構えも現在の姿に合わせます。
- 行動順、ストーリングによる増援の危険、退却確率を表示します。行動順と退却の成否は初期状態でオンです。中央のタイトルをクリックしてオフにすると、退却は確率だけになります。タイトルにマウスを合わせると遠征メーターが開きます。

#### マップと探索

- 部屋・通路・キュリオ・トラップ・障害物・戦闘・空腹マスを表示します。初期状態では判明した範囲だけを表示し、霧をオフにすると全体を見られます。クエスト用キュリオ・ボス・呪われた庭園への経路は、鍵と施錠された扉の順序も考慮します。
- 下段のカウンターで残りのマスを、補給品のアイコンで使い道を確認できます。戦闘・空腹アイコンから、未訪問マスの敵編成と空腹マスの表示を個別に隠せます。偵察確率、明るさの補正、特殊エンカウントの位置や出現条件も表示します。
- ゲームでキュリオ・障害物・空腹の画面が開くと、対応するカードが現れます。列をクリックするとゲームの選択肢を実行し、キュリオのアイテム列ならそのアイテムを使います。補給品が足りない列は実行しません。
- 偵察済みトラップの手前での自動停止は初期状態でオンです。トラップのカウンターでオフにできます。自動解除はしません。カードで英雄を選ぶと、その英雄で解除を試みます。
- 探索待機中にバッグか[I]を押すと、同じ品目をまとめて並べ直します。クエストアイテムはそのまま、空き枠は末尾に置きます。戦闘後は、戦利品画面を閉じて探索に戻った時点でデフォルトの整列順に自動で戻します。初期状態はオンで、パーティーのボタンでオフにできます。

#### 記録と村での準備

- アクティビティ・ログは戦闘・探索・キャンプの記録を続け、[End]で開けます。戦闘開始時にログへ自動で切り替わることはありません。セーブごとに直近10回の遠征と最終メーターを振り返れます。
- 村の英雄表ではレベル・遠征回数・歩数と、アプリが記録した累計値を比較できます。肖像にマウスを合わせると装備・戦闘スキル・キャンプスキルを表示します。
- 補給品の表はダンジョンと遠征の長さに応じたおすすめ数を示します。有効にしたダンジョンMOD（Courtyard Plus・Farmstead Plus・The Sunward Isles・Vermintide・The Fiend Festival）のダンジョンも表示し、選んだクエストの行を強調してそのダンジョンを表の一番上に移します。行をクリックして購入・売却・費用を確認し、**6秒以内に同じ行をもう一度クリックすると実行**します。数量に幅があれば上限に合わせ、無料支給品は売りません。赤の呪いを受けた英雄のための血も調整し、村に残る消耗状態の英雄の分を確保します。
- 図鑑では敵・トリンケット・村のイベント・病気・徳・精神崩壊・奇癖を、名前・レア度・クラス・効果で検索できます。建物・区画の画面では、選んだ強化に必要な資源と所持量を比較できます。計画用の機能で、ゲーム内で代わりに建設するものではありません。

</details>

### 導入

1. [最新リリース](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest)から`AncestorsMap.zip`をダウンロードし、任意のフォルダーに展開します。
2. `AncestorsMap.exe`を実行します。**.NET 8 Desktop Runtime**がなければ、インストールの案内が表示されます。
3. ゲームを起動するとセーブを自動で探します。初めて使うときは、右上のはてなマークから画面ガイドを開いてみてください。

### 動作環境・互換性

- Windows 10/11、[.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0)、インストール済みのDarkest Dungeon 1が必要です。アプリ本体は約**5.7MB**の実行ファイル1つで、ランタイムは別途必要です。
- リアルタイム情報と操作補助は、対応する**64ビット版**のゲームで使えます。Steam公開版・`coming_in_hot`ベータのSteam用およびDRMフリー用（`_windowsnosteam`）実行ファイルに対応しています。32ビット版や未対応のバージョンではメモリを読まず、セーブに基づく機能だけを使い、ログの状態欄に理由を表示します。
- 有効なDLC・MODと適用順を読み取ります。ダンジョン追加MODはCourtyard Plus、Farmstead Plus、The Sunward Isles、Vermintide、The Fiend Festivalで確認しています。すべてのMODを検証したわけではありません。
- Steamのインストールを基準とし、DRMフリー実行ファイルでも確認しています。GOGなどではインストール先やセーブの場所を自動検出できない場合があります。
- 한국어・English・日本語・简体中文に対応しています。初回はゲームの言語を使い、その後はアプリで選んだ言語を使います。

### 安全性

- **ゲームファイル・セーブ・ゲームメモリに直接書き込まず、ゲームのプロセスにコードを注入しません。** メモリは読み取り権限だけで開きます。アプリ自身の設定と遠征記録は別に保存します。
- **操作補助は実際にゲームを操作します。** 部屋の移動、カードの選択とアイテム使用、トラップ解除、自動購入、所持品整理、整列は、クリック・キー・ドラッグ入力を送ります。その結果はゲームの通常のセーブに反映されることがあります。
- トラップ手前の自動停止では、移動キーやマウスボタンを離す入力を送り、移動キーのリピート入力を止めます。**初期状態はオン**で、トラップのカウンターから切り替えます。戦闘後の自動整列も**初期状態はオン**で、パーティーのボタンで切り替えます。
- バッグにマウスを合わせて売却額を見るときも、探索中にゲームがマップタブを開いていれば、[Tab]入力で所持品タブを開きます。表示のために入力を送る場合もあります。
- 自動購入・整理中はマウスを動かさないでください。整理時は[Shift]を押さないでください。ゲームの破棄操作と重なるため、アプリはドラッグを行いません。
- 通信はGitHubのリリース確認に使います。起動時に自動で確認し、アプリ情報から手動でも確認できます。アカウントやAPIキーは不要で、ゲームの記録をアップロードしません。
- 他のプログラムのメモリを読むため、一部のウイルス対策ソフトが誤検知する場合があります。ダウンロードしたファイルはリリースに記載されたSHA-256で確認できます。

### 更新

新しいバージョンがあれば起動時に知らせます。左上の署名をクリックすると現在のバージョンと更新確認が表示されます。新しいバージョンの案内からリリースページを開き、zipをダウンロードしてください。自動ダウンロード・置き換えは行いません。アプリを終了してから新しいファイルを上書きします。設定と遠征記録は`%LocalAppData%\AncestorsMap`に残ります。

### 操作

| キー・マウス | 操作 |
|---|---|
| <code>[`]</code>または非表示ボタン | ろうそくのボタンだけを残す。ろうそくをクリックするか同じキーで再表示 |
| [Backspace] | 基本画面へ：村の英雄表／補給品表／探索マップ／戦闘画面 |
| [Home]／[End] | 図鑑／アクティビティ・ログを開く・閉じる |
| [Caps Lock] | 今すぐデフォルトの整列順に戻す |
| [I]またはバッグをクリック | 探索待機中に所持品を整理 |
| バッグにマウスを合わせる | ゲームの所持品・開いている戦利品の枠に売却額 |
| パーティーのアイコンをクリック | 戦闘後の自動整列のオン・オフ |
| 左ドラッグ／右ドラッグ | アプリの移動／マップの移動 |
| ホイール／ホイールクリック | マップの拡大・縮小／霧のオン・オフ |
| アプリのマップで隣接する部屋をクリック | 部屋にいるとき、その部屋へゲーム内で移動 |
| 自動表示されたカードの列をクリック | キュリオ・障害物・空腹の選択、または英雄を選んでトラップ解除 |
| 補給品の行をクリック→6秒以内に同じ行 | 購入内容の確認→自動購入 |
| ウィンドウの端をドラッグ／上部スライダー | サイズ／背景の不透明度 |
| はてなマーク／署名にマウスを合わせる・クリック | 画面ガイド／操作一覧・アプリ情報 |

ゲーム上のショートカットは、ゲームウィンドウが前面にあるときに動きます。[I]は探索待機中だけアプリが受け取り、それ以外はゲーム本来の操作になります。アプリ側でも<code>[`]</code>・[Home]・[End]を使えます。検索欄に文字があるときの[Backspace]は文字を消します。購入・整理はゲームを前面に出して行い、部屋の移動・カードの選択・トラップ解除などもゲームが前面にある必要があります。

### 画面ガイド

はてなマークから、使い始め、マップ、探索中の選択、戦闘、遠征管理、村での準備、記録と検索を確認できます。最初の6章は録画した見本の場面なので、ゲームを起動しなくても見られます。最後の「記録と調べもの」は利用者のデータを開きます。マウスを合わせられるステップでは金色の枠の中を試してください。暗い部分をクリックするかアプリを隠すと、ガイドを閉じます。

### 制限事項

- 敵の編成、空腹マス、行動順、退却の成否など、ゲームが隠している情報も表示します。必要な項目だけ有効にしてください。
- ゲームの更新後は、対応を確認するまでリアルタイム機能を使えません。セーブに基づく一部の表示は、ゲームが保存するまで遅れることがあります。
- おすすめ補給品はWiki・攻略情報・ダンジョン生成ルールを参考にしています。MODダンジョンには計算による推定値も含みます。パーティーや探索の予定に合わせて調整してください。
- 操作補助はゲーム画面と配置に依存します。未対応の配置や一部のMODでは機能が制限される場合があります。

### 不具合の報告

[Issues](https://github.com/Eolaloe/DD-AncestorsMap/issues)に、アプリのバージョン（署名をクリック）、ゲームのバージョン（公開版／`coming_in_hot`／DRMフリー版）、有効なMOD、どの画面で何をしたかを書いてください。可能ならスクリーンショットとアプリに表示された通知文も添えてください。

### ライセンス・クレジット

[LICENSE](LICENSE) — 個人での利用は自由。共有は公式リポジトリのリンクで(ファイルの再アップロード・改変版は要相談)。販売禁止。
Darkest Dungeon は Red Hook Studios のゲームです。
Claude と Codex の助けを借りて作りました。

</details>

<details>
<summary><img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1e8-1f1f3.png" width="20" alt="🇨🇳"> <b>简体中文说明</b></summary>

这是一个在《暗黑地牢》1游戏画面上显示**地图、战斗信息和活动日志**的悬浮工具。

即使游戏全屏也会始终置顶显示，点击工具窗口也不会抢走输入，操作仍然由游戏接收。**建议将其叠放在游戏画面上使用。**

工具里没有写死任何原版数据。它会**按照加载顺序读取当前存档所启用的本体、DLC 和所有模组的数据并合并**，因此模组新增或修改的奇物、敌人、饰品和特质，也会按游戏内的实际数值显示。名称与说明采用游戏译文，读取另一个存档时会自动重新同步。在图鉴搜索框中输入文字时，键盘输入交给工具。

<p align="center">
<img src="images/anim_battle.zh.webp" width="49%" alt="切换战斗技能后，各目标的伤害与效果数值随之变化">
<img src="images/anim_map.zh.webp" width="49%" alt="鼠标悬停在格子上即可显示卡片">
</p>

### 主要功能

- **战斗界面**——在目标上方显示所选技能的伤害、命中、暴击和效果概率，也能查看队友支援、位移、敌人选定的技能与目标，以及当前状态和下次行动的持续效果。
- **探索中的选择**——在奇物、障碍物和饥饿卡片中查看结果并执行选项。陷阱卡片列出各英雄的解除概率与压力，供你选择由谁尝试解除。
- **陷阱前自动停步与物品整理**——在已侦察到的陷阱前停步；点击背包或按[I]整理物品。将鼠标移到背包上，可在游戏的物品栏和战利品格中显示售价。
- **详细地图**——查看奇物结果、敌人组成、剩余格数、补给用途、目标路线，以及侦察概率和亮度修正。
- **记录与城镇准备**——提供活动日志、统计面板、英雄表、图鉴搜索、补给推荐（含地牢模组）与自动购买，以及建筑升级与区域建筑所需资源的计算。
- **界面指南**——点击问号打开7章、31步的引导。说明使用预先录制的示例场景，部分步骤还可以移入鼠标查看卡片。

### 界面示例

<table>
<tr><td align="center" width="50%"><img src="images/card_curio.zh.webp" alt="比较徒手和使用钥匙的结果并执行选择的奇物卡片"><br><sub>奇物卡片</sub></td><td align="center" width="50%"><img src="images/card_trap.zh.webp" alt="各英雄的陷阱解除概率与压力"><br><sub>解除陷阱</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/heroes.zh.webp" alt="城镇英雄表及装备和技能卡片"><br><sub>英雄表与卡片</sub></td><td align="center" width="50%"><img src="images/supplies.zh.webp" alt="按地牢和远征长度列出的补给推荐表"><br><sub>补给推荐</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/meter.zh.webp" alt="比较各英雄远征数据的统计面板"><br><sub>远征统计</sub></td><td align="center" width="50%"><img src="images/codex.zh.webp" alt="图鉴搜索与敌人卡片"><br><sub>图鉴</sub></td></tr>
</table>

### 功能详情

<details>
<summary>展开各项功能说明</summary>

#### 战斗

- 进入战斗后，主界面会从地图切换为战斗界面。己方行动时，显示所选技能可作用目标的数值；敌方行动时，只显示敌人已选定目标的数值。治疗、增益和位移技能也会按相应阵型展示。
- 角色上方的两列分别显示已有状态及剩余时间、下次行动的持续效果量。预计持续伤害会耗尽生命时，以血迹提示。角色下方显示当前生命和压力。
- 将鼠标移到下方头像上，可打开英雄或敌人的战斗卡片，比较计入当前装备、特质、疾病、增益及触发条件后的数值，以及敌人选择技能和目标的概率。外观也会跟随当前皮肤、变身或姿态。
- 显示行动顺序、拖延战斗带来的增援风险和撤退概率。行动顺序与撤退结果默认开启，点击中央标题可关闭；关闭后，撤退只显示概率。将鼠标移到标题上可打开远征统计面板。

#### 地图与探索

- 显示房间、走廊、奇物、陷阱、障碍物、战斗和饥饿格。默认只显示已知区域，关闭迷雾后可查看全图。任务奇物、首领和庭院的路线会考虑钥匙与锁门的先后顺序。
- 下方计数器显示剩余格子，补给图标显示该物品的用途。战斗与饥饿图标可分别隐藏未到访格子的敌人组成和饥饿格。还可查看侦察概率、亮度修正，以及特殊遭遇的位置或出现条件。
- 游戏打开奇物、障碍物或饥饿窗口时，工具会显示对应卡片。点击列即可执行游戏选项；点击奇物的物品列会使用相应物品。补给不足的列不会执行。
- 已侦察陷阱前的自动停步默认开启，可点击陷阱计数器关闭。工具不会自动解除陷阱；需要在卡片中选择英雄，由该英雄尝试解除。
- 探索待机时点击背包或按[I]，会合并同类堆叠并整理顺序。任务物品留在原位，空格移到末尾。战斗后，关闭战利品窗口、返回探索时会自动恢复初始队伍阵型；此功能默认开启，可通过队伍按钮关闭。

#### 记录与城镇准备

- 活动日志持续记录战斗、探索和扎营事件，按[End]打开。进入战斗不会自动切换到日志。每个存档保留最近10次远征及其最终统计，供以后查看。
- 城镇英雄表可比较等级、远征次数、步数和工具记录的累计数值。将鼠标移到头像上，可查看装备、战斗技能和扎营技能。
- 补给表按地牢和远征长度给出推荐数量。已启用的地牢模组（Courtyard Plus、Farmstead Plus、The Sunward Isles、Vermintide、The Fiend Festival）的地牢也会列出，并高亮所选任务的行，把该地牢移到表格最上方。点击一行预览购买、出售和费用，**6秒内再次点击同一行即可执行**。数量范围按上限处理，不会出售免费发放的物品。还会为受猩红诅咒的英雄调整血酿数量，并为留在城镇中处于凋零状态的英雄留出份额。
- 图鉴可按名称、品质、职业和效果搜索敌人、饰品、城镇事件、疾病、美德、折磨与特质。建筑与区域建筑界面可比较所选升级需要的资源与持有量；它只用于规划，不会替你在游戏里建造。

</details>

### 安装

1. 从[最新发行版](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest)下载`AncestorsMap.zip`，解压到任意文件夹。
2. 运行`AncestorsMap.exe`。如果没有安装**.NET 8 Desktop Runtime**，会出现安装提示。
3. 启动游戏后，工具会自动查找存档。首次使用建议点击右上角问号，查看界面指南。

### 要求与兼容性

- 需要Windows 10/11、[.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0)和已安装的《暗黑地牢》1。工具本体为约**5.7MB**的单个exe，运行时需另行安装。
- 实时信息与输入辅助需要受支持的**64位**游戏。支持Steam公开版和`coming_in_hot`测试版的Steam及无DRM（`_windowsnosteam`）执行文件。32位或未识别的游戏版本不会读取内存，只提供基于存档的功能，并在日志状态栏说明原因。
- 会读取启用的DLC、模组及其加载顺序。已确认的地牢模组包括Courtyard Plus、Farmstead Plus、The Sunward Isles、Vermintide和The Fiend Festival，并非所有模组都经过验证。
- 以Steam安装方式为基准，也确认过无DRM执行文件。GOG等其他平台的安装位置或存档路径可能无法自动识别。
- 支持한국어、English、日本語和简体中文。首次启动跟随游戏语言，此后使用你在工具中选择的语言。

### 安全说明

- **不会直接写入游戏文件、存档或游戏内存，也不会向游戏进程注入代码。** 内存仅以读取权限打开。工具自身的设置与远征记录另行保存。
- **输入辅助会实际操作游戏。** 房间移动、卡片选项和物品使用、陷阱解除、自动购买、物品整理及阵型恢复，都会发送点击、按键或拖放输入。这些操作的结果可能由游戏正常写入存档。
- 陷阱前自动停步会发送松开移动键或鼠标按钮的输入，并拦截移动键的重复输入。此功能**默认开启**，通过陷阱计数器切换。战斗后自动恢复阵型同样**默认开启**，通过队伍按钮关闭。
- 将鼠标移到背包上查看售价时，如果探索中的游戏正显示地图标签，也会发送[Tab]来打开物品栏。因此，部分显示功能也会发送输入。
- 自动购买或整理时请勿移动鼠标。整理时也请勿按住[Shift]；这会与游戏的丢弃操作冲突，工具因此不会执行拖放。
- 联网用于查询GitHub发行版：启动时自动检查，也可在应用信息中手动检查。不需要账号或API密钥，不会上传游戏记录。
- 读取其他程序内存可能触发部分杀毒软件的误报。可使用发行说明提供的SHA-256核对下载文件。

### 更新

有新版本时，启动工具会出现提示。点击左上角署名可查看当前版本并检查更新。在新版本提示中打开发行页面，下载新zip即可。工具不会自动下载或替换文件；请先关闭正在运行的工具，再覆盖文件。设置与远征记录保存在`%LocalAppData%\AncestorsMap`。

### 操作

| 按键或鼠标 | 功能 |
|---|---|
| <code>[`]</code>或隐藏按钮 | 只留下蜡烛按钮；点击蜡烛或再次按键恢复 |
| [Backspace] | 返回主界面：城镇英雄表／补给表／探索地图／战斗界面 |
| [Home]／[End] | 打开或关闭图鉴／活动日志 |
| [Caps Lock] | 立即恢复初始队伍阵型 |
| [I]或点击背包 | 探索待机时整理物品栏 |
| 将鼠标移到背包上 | 显示游戏物品栏及已打开战利品格的售价 |
| 点击队伍图标 | 切换战斗后自动恢复阵型 |
| 左键拖动／右键拖动 | 移动工具窗口／移动地图 |
| 滚轮／中键单击 | 缩放地图／切换迷雾 |
| 点击工具地图上相连的房间 | 身处房间时，在游戏中前往该房间 |
| 点击自动弹出卡片中的列 | 执行奇物、障碍物、饥饿选项，或选择英雄解除陷阱 |
| 点击补给行→6秒内再次点击同一行 | 预览购买→自动购买 |
| 拖动窗口边缘／顶部滑块 | 调整尺寸／背景不透明度 |
| 问号／鼠标移到署名上或点击署名 | 界面指南／操作说明或应用信息 |

游戏上的快捷键在游戏窗口位于前台时生效。[I]仅在探索待机时由工具接管，其他时候保留游戏原本的功能。在工具窗口中也可使用<code>[`]</code>、[Home]和[End]；搜索框有文字时，[Backspace]会删除文字。购买和整理会将游戏切到前台，房间移动、卡片选择、陷阱解除等也需要游戏窗口位于前台。

### 界面指南

点击问号，可依次了解初次使用、地图、探索选择、战斗、远征管理、城镇准备，以及记录与查阅。前6章使用录制好的示例场景，不启动游戏也能查看；最后的“记录与查阅”会打开用户自己的数据。允许悬停的步骤可以将鼠标移入金色边框。点击暗处或隐藏工具即可关闭指南。

### 已知限制

- 敌人组成、饥饿格、行动顺序和撤退结果等信息包含游戏原本隐藏的内容。请按需要启用。
- 游戏更新后，在确认兼容前无法使用实时功能。部分基于存档的信息要等游戏保存后才会更新。
- 补给推荐参考了Wiki、攻略和地牢生成规则，模组地牢还包含计算估值。请根据队伍与探索计划调整。
- 输入辅助依赖游戏画面和布局；不支持的布局或某些模组可能限制功能。

### 问题反馈

请在[Issues](https://github.com/Eolaloe/DD-AncestorsMap/issues)中说明工具版本（点击署名查看）、游戏版本（公开版／`coming_in_hot`／无DRM版）、启用的模组，以及在哪个界面进行了什么操作。方便的话，请附上截图和工具显示的通知文字。

### 许可与致谢

[LICENSE](LICENSE) — 可自由用于个人用途；请通过官方仓库链接分享（重新上传文件或发布修改版请先联系作者）；禁止售卖。
《暗黑地牢》（Darkest Dungeon）是 Red Hook Studios 的游戏。
在 Claude 和 Codex 的协助下制作。

</details>

---

<img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1fa-1f1f8.png" width="20" alt="🇺🇸"> <b>English</b>

An overlay for Darkest Dungeon 1 that puts **maps, combat information and an activity log** over the game.

It stays on top even over a fullscreen game, and clicking it doesn't steal your input — the game keeps receiving it. **Using it on top of the game screen is recommended.**

Nothing is hard-coded from vanilla. It **reads the base game, DLC and every mod enabled in your current save in their load order and merges them**, so curios, monsters, trinkets and quirks added or changed by mods show up with their real in-game values. Names and descriptions use the game's translations, and loading a different save re-syncs on its own. Typing in the Codex search box gives keyboard focus to the app.

<p align="center">
<img src="images/anim_battle.en.webp" width="49%" alt="Per-target damage and effect values changing as different combat skills are selected">
<img src="images/anim_map.en.webp" width="49%" alt="Hover a tile to see its card">
</p>

### What it does

- **Battle screen** — See damage, hit, crit and effect chances above each target of your selected skill. It also shows support skills, movement, the enemy's chosen skill and targets, active statuses and effects due next turn.
- **Exploration choices** — Check the outcomes on curio, obstacle and hunger cards, then click an option. Trap cards let you compare each hero's disarm chance and stress before choosing who should try.
- **Trap stopping and inventory sorting** — Stop before scouted traps, and sort supplies and loot with the bag button or `[I]`. Hover over the bag to display sell values on the game's inventory and loot slots.
- **Detailed map** — Check curio outcomes, enemy groups, remaining tiles, supply uses, routes to objectives, scouting chance and light modifiers.
- **Records and town preparation** — Use the activity log, meters, hero table, Codex search, supply recommendations (dungeon mods included), auto-buy and building or district cost planner.
- **Screen guide** — Open a seven-chapter, 31-step tour from the question-mark button. It uses recorded example scenes, with cards you can hover over in some steps.

### Screenshots

<table>
<tr><td align="center" width="50%"><img src="images/card_curio.en.webp" alt="A curio card with clickable columns for bare-handed interaction and using a key"><br><sub>Curio card</sub></td><td align="center" width="50%"><img src="images/card_trap.en.webp" alt="Trap disarm chances and stress for each hero"><br><sub>Trap disarming</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/heroes.en.webp" alt="The town hero table with an equipment and skills card"><br><sub>Hero table and card</sub></td><td align="center" width="50%"><img src="images/supplies.en.webp" alt="Recommended provisions by dungeon and expedition length"><br><sub>Supply recommendations</sub></td></tr>
<tr><td align="center" width="50%"><img src="images/meter.en.webp" alt="An expedition meter comparing each hero's contributions"><br><sub>Expedition meter</sub></td><td align="center" width="50%"><img src="images/codex.en.webp" alt="Codex search with an enemy card"><br><sub>Codex</sub></td></tr>
</table>

### In detail

<details>
<summary>Expand the feature descriptions</summary>

#### Combat

- When combat starts, the main view changes from the map to the battle screen. On a hero's turn, it shows values for the targets their selected skill can reach. On an enemy's turn, it shows values for the targets the enemy has already chosen. Healing, buffs and movement skills use the appropriate formation.
- Two columns above each character distinguish active statuses and their remaining duration from ongoing effect amounts due next turn. A blood splatter marks expected HP depletion from ongoing damage. Current HP and stress appear below the character.
- Hover over the portraits along the bottom for hero and enemy combat cards. Compare values based on current equipment, quirks, diseases, buffs and conditions, as well as enemy skill and target selection chances. Artwork follows the current skin, transformation or stance.
- Check turn order, stalling reinforcement risk and retreat chance. Turn order and the predicted retreat result are on by default. Click the central title to hide them; retreat then shows only its chance. Hover over the title to open the expedition meter.

#### Map and exploration

- View rooms, corridors, curios, traps, obstacles, battles and hunger tiles. Fog is on by default, showing revealed areas only; turn it off to see the whole map. Routes to quest curios, bosses and through the Courtyard account for keys and locked doors.
- The bottom counters show remaining tiles, while supply icons show where each item can be used. The battle and hunger icons separately hide enemy groups in unvisited tiles and hunger tile markers. You can also check scouting chance, light modifiers and special encounter locations or spawn conditions.
- Opening a curio, obstacle or hunger window in the game brings up the matching card. Click a column to execute that choice in the game; an item column on a curio card uses the item. Columns that require more supplies than you have will not execute.
- Automatic stopping before scouted traps is on by default. Toggle it with the trap counter. It does not disarm traps automatically: choose a hero on the card to attempt the disarm.
- While idle in a dungeon, click the bag or press `[I]` to merge stacks and arrange your inventory. Quest items stay in place and empty slots move to the end. After combat, the default party order is restored automatically once the loot window closes and exploration resumes. This is on by default; turn it off with the party button.

#### Records and town preparation

- The activity log keeps recording combat, exploration and camping events. Open it with `[End]`; combat no longer opens the log automatically. Review the last ten expeditions for each save, including their final meters.
- The town hero table compares levels, expedition counts, steps and cumulative stats recorded by the app. Hover over a portrait for equipment, combat skills and camping skills.
- The provisions table recommends amounts by dungeon and expedition length. Dungeons from enabled dungeon mods (Courtyard Plus, Farmstead Plus, The Sunward Isles, Vermintide, The Fiend Festival) are listed too, and the quest you picked is highlighted with its dungeon moved to the top. Click a row to preview purchases, sales and cost, then **click the same row again within six seconds to proceed**. Ranges use the higher amount, and free provisions are not sold. It also adjusts Blood for cursed party members while reserving Blood for wasting heroes left in town.
- Search the Codex for enemies, trinkets, town events, diseases, virtues, afflictions and quirks by name, rarity, class or effect. The building and district view compares planned upgrade costs with your resources. It is a planner, not an automatic building tool.

</details>

### Installation

1. Download `AncestorsMap.zip` from the [latest release](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest) and extract it to any folder.
2. Run `AncestorsMap.exe`. If the **.NET 8 Desktop Runtime** is missing, an installation prompt appears.
3. Launch the game and the app finds your save automatically. On your first run, try the question-mark button in the top-right corner.

### Requirements & compatibility

- Windows 10/11, the [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0) and an installed copy of Darkest Dungeon 1. The app is a single executable of about **5.7 MB**; the runtime is separate.
- Live information and input assistance require a supported **64-bit** game build. The Steam public and `coming_in_hot` beta builds are supported, with either the Steam or DRM-free (`_windowsnosteam`) executable. With a 32-bit or unrecognised build, the app skips memory reading, offers save-based features only, and explains why in the log's status line.
- Active DLC, mods and their load order are read from your save. Dungeon mods checked include Courtyard Plus, Farmstead Plus, The Sunward Isles, Vermintide and The Fiend Festival. Not every mod has been tested.
- Built around Steam installations and also checked with the DRM-free executable. Other platforms, including GOG, may use game or save locations the app cannot find automatically.
- Supports 한국어, English, 日本語 and 简体中文. It follows the game language on first run, then uses the language you choose in the app.

### Safety

- **The app does not write directly to game files, saves or game memory, or inject code into the game process.** It opens memory with read permissions only. Its own settings and expedition records are stored separately.
- **Input assistance does operate the game.** Room movement, card choices and item use, trap disarming, auto-buy, sorting and party reordering send clicks, keystrokes or drag-and-drop input. The game may save the results of these actions normally.
- Automatic trap stopping sends key or mouse-button releases and blocks repeated movement-key input. It is **on by default**, controlled by the trap counter. Automatic party reordering after battle is also **on by default**, controlled by the party button.
- Even hovering over the bag for sell values can send `[Tab]` to open the inventory if the game is showing its map tab during exploration. Some display features therefore also send input.
- Do not move the mouse during auto-buy or sorting. Do not hold `[Shift]` while sorting: it overlaps with the game's discard action, so the app will not perform the drag.
- Network access is used to check GitHub releases: automatically at startup, or manually from app info. No account or API key is needed, and game records are not uploaded.
- Reading another process's memory may trigger antivirus false positives. Use the SHA-256 provided with the release to verify your download.

### Updates

The app checks for a new version at startup. Click the signature in the top-left corner to see your version or check again. A new-version notice links to the release page, where you can download the new zip. Nothing is downloaded or replaced automatically. Close the running app before overwriting its files. Settings and expedition records remain in `%LocalAppData%\AncestorsMap`.

### Controls

| Key or mouse action | What it does |
|---|---|
| <code>[`]</code> or the hide button | Leave only the candle button; click the candle or press the key again to return |
| `[Backspace]` | Return to the main view: town heroes / provisions / dungeon map / battle screen |
| `[Home]` / `[End]` | Open or close the Codex / Activity Log |
| `[Caps Lock]` | Restore the default party order now |
| `[I]` or click the bag | Sort inventory while idle in a dungeon |
| Hover over the bag | Show sell values on game inventory and open loot slots |
| Click the party icon | Toggle automatic party reordering after battle |
| Left-drag / right-drag | Move the app window / pan the map |
| Mouse wheel / middle-click | Zoom the map / toggle fog |
| Click a connected room on the app map | Move there in the game while standing in a room |
| Click a column on an automatic card | Choose a curio, obstacle or hunger option, or select a hero to disarm a trap |
| Click a supply row, then again within six seconds | Preview the purchase, then auto-buy |
| Drag a window edge / top slider | Resize / adjust background opacity |
| Question mark / hover over or click the signature | Screen guide / controls list or app info |

Shortcuts over the game work while its window is active. The app takes `[I]` only while idle in a dungeon; otherwise it retains its game function. In the app itself, <code>[`]</code>, `[Home]` and `[End]` also work; `[Backspace]` deletes text when the search field contains any. Buying and sorting bring the game to the front. Room movement, card choices and trap disarming also require the game window to be active.

### Screen guide

Use the question mark to explore getting started, the map, exploration choices, combat, expedition management, town preparation, and records and reference. The first six chapters use recorded example scenes, so you can view them without running the game. The final chapter opens your own records and reference views. In steps that allow hovering, try the areas inside the gold outlines. Click a darkened area or hide the app to close the guide.

### Known limitations

- The app can reveal information the game hides, including enemy groups, hunger tiles, turn order and retreat results. Enable only the information you want.
- After a game update, live features are unavailable until support for that build is confirmed. Some save-based displays can lag until the game saves.
- Provisions recommendations draw on wikis, guides and dungeon generation rules; mod dungeon values include calculated estimates. Adjust them for your party and exploration plans.
- Input assistance depends on the game screen and layout. Unsupported layouts or some mods may limit these features.

### Reporting issues

Open an [issue](https://github.com/Eolaloe/DD-AncestorsMap/issues) with your app version (click the signature), game version (public / `coming_in_hot` / DRM-free), active mods, and which screen and action caused the problem. Include a screenshot and the app's notification text if possible.

### License & credits

[LICENSE](LICENSE) — free for personal use; share the official repository link (ask before re-uploading the file or sharing a modified build); no selling.
Darkest Dungeon is a game by Red Hook Studios.
Made with help from Claude and Codex.
