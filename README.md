# Ancestor's Map — DD Field Guide

**[⬇ Download / 다운로드 / ダウンロード / 下载](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest)**

<details>
<summary><img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1f0-1f1f7.png" width="20" alt="🇰🇷"> <b>한국어</b> — 다키스트 던전 상세 지도 · 전투 정보 · 활동 일지 오버레이</summary>

다키스트 던전 1을 하는 동안 **게임이 보여 주지 않는 상세 던전 지도 · 전투 정보 · 활동 일지**를 게임 화면 위에 띄워 주는 오버레이입니다.
항상 최상위 창으로 떠서 전체화면 게임 위에 겹쳐지고, 앱을 클릭해도 입력은 게임이 그대로 받습니다.

바닐라 정보를 고정으로 넣어 둔 것이 아닙니다. **지금 불러온 세이브에 켜진 본편 + DLC + 모드 데이터를 읽어 병합**하므로, 모드가 추가하거나 바꾼 골동품 · 적 · 장신구 · 기벽도 실제 인게임 값 그대로 보입니다. 다른 세이브를 불러오면 알아서 다시 맞춥니다.

### 무엇이 되나

- **상세 지도** — 인게임 지도와 같은 꼴에 골동품 · 함정 · 적 구성 · 상호작용 결과를 마우스 호버로. 퀘스트 골동품 · 보스 · 안뜰의 **최단 경로 안내**, 아직 남은 골동품의 **보급품 트래커**, 정찰 확률, 밝기 보정 수치, 특수 조우(별에서 온 존재 · 광신도 · 기는 혼돈 · 수집가) 안내.
- **전투 정보** — 각 자리에서 쓸 수 있는 기술의 명중 · 피해 · 치명 · 효과 확률, 적의 기술 · 대상 선택 확률, 턴 순서, 스톨링(증원 방지 횟수 · 다음 라운드 예고), 후퇴 판정.
- **활동 일지 · 미터기** — 전투 · 탐험 · 야영 기록이 자동으로 쌓이고, 영웅별 처치 · 입힌 피해 · 입은 피해 · 회복 · 스트레스를 막대그래프로 비교.
- **도감 검색** — 적 · 장신구 · 마을 이벤트 · 질병 · 각성 · 붕괴 · 기벽을 이름 · 등급 · 직업 · 효과 어떤 값으로든. 모드 항목도 같이.
- **마을에서** — 던전 · 길이별 **추천 보급품**, 건물 증축 · 추가 건물 **요구 재화 계산**(보유량 + 이번 원정 획득분 대비).
- **화면 안내** — 오른쪽 위 물음표(?) 단추를 누르면 각 화면을 단계별로 짚어 설명합니다(마을에서도 샘플 원정으로).

일부 기능은 게임이 의도적으로 감추는 정보를 보여 줍니다. 지도는 기본으로 **탐색한 곳만** 보이고 전체 보기는 상단 단추로 켭니다. 턴 순서와 후퇴 성공 여부는 기본으로 켜져 있고, 전투 막대 가운데 타이틀을 눌러 끌 수 있습니다.

#### 지도
- 인게임 지도와 비슷한 모양의 상세 지도. 탐색한 곳만 볼지, 전체를 볼지 고를 수 있습니다.
- 남은 전투 · 골동품 · 함정 · 허기짐 칸 수와, 골동품에 쓸 보급품이 몇 개 필요한지 알려줍니다.
- 칸에 마우스를 올리면 적 구성, 골동품에 쓸 보급품과 결과, 함정과 장애물의 효과, 허기짐 활성 여부, 비밀방을 볼 수 있습니다.
- 핏빛 궁정 안뜰 대서사시 지도도 지원합니다.

#### 길 안내 · 특수 인카운터 · 밝기
- 퀘스트 골동품, 보스, 안뜰 대서사시까지 **가장 짧은 길**을 안내합니다.
- 별에서 온 존재와 광신도는 지도에서 **위치를 짚어 주고**, 수집가와 기는 혼돈은 **등장 조건과 확률**을 알려줍니다.
- 밝기에 따라 달라지는 스트레스, 정찰, 기습, 회피, 치명타, 적 명중과 피해, 추가 전리품 보정을 **정확한 수치**로 보여줍니다.

#### 전투
- 이번 라운드 아군과 적의 **턴 순서**, 그리고 지금 누구 차례인지.
- 초상에 마우스를 올리면 **전투 카드**가 뜹니다.
  - 아군은 적 각 열을 칠 때의 명중, 피해, 치명타, 효과 확률 — 장신구 · 기벽 · 질병 · 버프를 모두 반영한 최종 성능이고, 게임이 따로 보여 주지 않는 숨은 보정까지 넣은 실제 명중률입니다.
  - 적은 아군 각 열을 칠 때의 같은 수치와 함께, 어떤 기술을 쓸지 · 누구를 노릴지의 확률.
  - 괴인이나 결투가처럼 모드가 바뀌는 캐릭터는 **지금 모드**의 모습과 기술로.
- **스톨링** — 다음 라운드에 증원이 올 위험을 색으로 알려주고, 이번 라운드에 증원 방지 행동을 몇 번 했는지 실시간으로 셉니다.
- **후퇴** — 성공 확률, 그리고 턴 순서를 켜 두면 지금 후퇴했을 때 성공할지 실패할지.
- **원정 미터기** — 가운데 타이틀에 마우스를 올리면 이번 원정에서 영웅마다 처치, 입힌 피해, 입은 피해, 체력 회복, 받은 스트레스, 스트레스 해소, 기절을 비교합니다. 야영 기술과 식사, 아이템 회복도 셉니다.

#### 활동 일지
- 전투와 탐험에서 일어난 일을 게임 용어와 색으로 기록합니다. 기술, 명중, 피해, 효과, 저항, 반격, 심장마비, 부가 행동부터 골동품, 함정, 장애물, 허기짐까지.
- 판정은 짐작하지 않고 **게임이 띄운 판정 결과**를 그대로 읽어 적습니다.
- 전투가 시작되면 자동으로 일지로, 끝나면 지도로 돌아갑니다.
- 던전 한 번이 일지 하나이고, 세이브마다 최근 10개를 남겨 두어 다시 볼 수 있습니다.

#### 마을
- 던전과 원정 길이에 맞는 **보급품 추천 수량**.
- **도감** — 적, 장신구, 마을 이벤트, 질병, 각성, 붕괴, 기벽을 어떤 값으로든 검색.
- **건물 증축 · 추가 건물 요구량** — 고른 단계에 필요한 재화를 보유량(영지 + 원정 중 획득)과 비교. 효과 설명은 인게임과 같고, 원정 중에도 열 수 있습니다.

### 설치

1. [Releases](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest) 에서 `AncestorsMap.zip` 을 받아 아무 폴더에 풉니다.
2. `AncestorsMap.exe` 를 실행합니다. **.NET 8 Desktop Runtime** 이 필요하며, 없으면 설치 안내 창이 뜹니다.
3. 게임을 켜면 세이브를 자동으로 찾습니다. 처음이면 물음표 단추로 화면 안내를 한 번 보세요.

### 요구 · 호환

- Windows 10/11, [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0).
- 게임을 **64비트로 실행**해야 실시간 정보(턴 순서 · 스톨링 · 후퇴 · 골동품 창)를 읽습니다. 스팀 공개판 · coming_in_hot 베타, 스팀 · DRM 없는(`_windowsnosteam`) 실행 파일을 지원합니다. 32비트거나 아직 모르는 게임 버전이면 메모리는 읽지 않고 **세이브만으로 동작**하며, 활동 일지 위 상태 줄에 이유가 뜹니다.
- 모드는 세이브에 적힌 활성 목록과 우선순위를 읽어 자동 반영합니다. 게임 데이터를 바꾸는 대부분의 모드와 함께 쓸 수 있습니다(던전 추가 모드는 Farmstead Plus, The Sunward Isles, Vermintide로 확인).
- 스팀판 기준으로 만들고 DRM 없는 실행 파일로도 확인했습니다. GOG 등 다른 플랫폼은 게임 경로 · 세이브 위치 인식이 다를 수 있습니다.
- 한국어 · English · 日本語 · 简体中文. 처음에는 게임 언어를 따라가고, 이름과 설명은 게임 번역을 그대로 씁니다.

### 안전

- 세이브 · 게임 파일 · 게임 메모리에 **아무것도 쓰지 않습니다.** 게임에 코드를 끼워 넣지도 않습니다(후킹 · 인젝션 없음).
- 메모리는 **읽기 권한으로만** 엽니다. 세이브는 한 턴 늦게 쓰이고 판정 결과는 세이브에 남지 않아서, 전투 중 실시간 값을 맞추는 데만 씁니다. 값을 찾아 **고치는** 치트 엔진과 달리, 찾아서 **보여 주기**만 합니다.
- 통신은 **시작할 때 새 버전 확인 한 번**(GitHub 릴리스 조회)뿐입니다. 계정 · 키 · 수집 없음.
- 다른 프로그램의 메모리를 읽는 특성상 일부 백신이 오탐할 수 있습니다. 받은 파일이 원본인지는 릴리스 노트의 SHA-256 으로 확인할 수 있습니다.
- 그림과 문구는 설치된 게임에서 읽습니다. 게임 자산을 포함하지 않으며, 프로그램은 실행 파일 하나(약 3.5MB)입니다.

### 업데이트

새 버전이 나오면 앱을 켤 때 안내 창이 뜨고, "업데이트 확인"을 누르면 이 저장소의 릴리스 페이지가 열립니다. 자동으로 내려받거나 교체하지는 않습니다 — 새 zip 을 받아 덮어쓰면 됩니다. 왼쪽 위 서명을 누르면 지금 버전과 업데이트 확인 단추가 있습니다. 설정과 원정 기록은 `%LocalAppData%\AncestorsMap` 에 남습니다.

### 조작

| 키 · 마우스 | 동작 |
|---|---|
| `` ` `` (Tab 위) | 보이기 · 숨기기 |
| `Caps Lock` | 게임의 **기본 원정대 설정** 단추 누르기 (게임에 단축키가 없는 기능) |
| `Home` | 도감 · 활동 일지 · 영지를 닫고 기본 화면(지도)으로 |
| 좌클릭 드래그 · 우클릭 드래그 | 창 이동 · 지도 이동 |
| 휠 · 휠 클릭 | 확대 · 축소 · 지도 ↔ 활동 일지 |
| 창 경계 드래그 · 상단 슬라이더 | 창 크기 · 투명도 |
| 물음표 단추 · 왼쪽 위 서명 | 화면 안내 · 앱 정보(버전 · 업데이트 확인) |

`` ` ``, `Caps Lock`, `Home`, 게임 위 휠 클릭은 **게임 화면이 앞에 있을 때만** 동작하고, 다른 프로그램에서는 원래대로 쓰입니다.

### 알려진 한계

- 실시간 정보는 지원하는 64비트 게임 버전에서만 읽습니다. 게임이 업데이트되면 앱이 새 버전에 맞춰질 때까지 세이브만으로 동작합니다.
- 추천 보급품 표는 영문 위키 · 공략 글 · 던전 생성 규칙 계산을 합친 참고값입니다.
- 모든 모드를 검증하지는 못했습니다. 이상하게 보이면 아래로 알려 주세요.

### 문제 신고

[Issues](https://github.com/Eolaloe/DD-AncestorsMap/issues) 에 아래를 함께 적어 주세요.
- 앱 버전(왼쪽 위 서명 클릭) · 게임 버전(스팀 공개판 / coming_in_hot / DRM 없는 판)
- 켜 둔 모드 목록 · 어느 화면에서 무엇을 했을 때인지 · 가능하면 스크린샷

### 라이선스 · 크레딧

[LICENSE](LICENSE) — 개인 사용 자유, 원본 그대로 출처를 밝힌 재배포만 허용, 판매 금지.
Darkest Dungeon 은 Red Hook Studios 의 게임이며, 이 앱은 게임 자산을 포함하지 않습니다.
Claude · ChatGPT 의 도움을 받아 만들었습니다.

</details>

<details>
<summary><img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1ef-1f1f5.png" width="20" alt="🇯🇵"> <b>日本語</b> — ダーケスト・ダンジョンの詳細マップ・戦闘情報・アクティビティログのオーバーレイ</summary>

ダーケスト・ダンジョンのプレイ中に、**ゲームが見せてくれない詳細なダンジョンマップ・戦闘情報・アクティビティログ**をゲーム画面の上に表示するオーバーレイです。
フルスクリーンのゲームの上にも常に最前面で重なり、アプリをクリックしても入力はそのままゲーム側に届きます。

バニラの情報を固定で埋め込んでいるわけではありません。**いまロードしているセーブで有効な本編・DLC・MODのデータを読み込んで統合する**ので、MODで追加・変更されたキュリオ・敵・トリンケット・奇癖も、実際のゲーム内の数値どおりに表示されます。別のセーブをロードしても自動で合わせ直します。

### できること

- **詳細マップ** — ゲーム内マップと同じ形。マスにマウスを乗せると、キュリオ・トラップ・敵の編成・調べたときの結果を表示します。クエスト用キュリオ・ボス・呪われた庭園への**最短ルート案内**、まだ調べていないキュリオに必要な**物資のトラッカー**、偵察確率、明るさによる補正値、特殊エンカウント（シング・フロム・ザ・スター、ファナティック、シャンブラー、コレクター）の案内も。
- **戦闘情報** — 各位置から使えるスキルの命中・ダメージ・クリティカル・効果の確率、敵がどのスキルを誰に使いそうか、行動順、戦闘の引き延ばし（ストーリング）の状況（このラウンドに増援を防ぐ行動を何回したか・次のラウンドに何が起きるか）、退却の判定。
- **アクティビティログ・メーター** — 戦闘・探索・キャンプの記録が自動で残り、英雄ごとの撃破数・与ダメージ・被ダメージ・回復・ストレスを棒グラフで比較できます。
- **データベース検索** — 敵・トリンケット・村のイベント・病気・徳・精神崩壊・奇癖を、名前・レア度・クラス・効果など、どんな値からでも検索できます。MODの項目も含みます。
- **村で** — ダンジョンと遠征の長さに応じた**おすすめ物資**、建物・区画の強化に必要な**資源の計算**（手持ち＋今回の遠征で得た分と比較）。
- **画面ガイド** — 右上の **?** ボタンを押すと、各画面を順を追って説明します（サンプルの遠征を使うので、村にいても見られます）。

一部の機能は、ゲームが意図的に隠している情報を表示します。マップは初期状態では**探索済みの場所だけ**を表示し、全体表示は上部のボタンで切り替えます。行動順と退却の成否は初期状態でオンになっていて、戦闘バー中央のタイトルをクリックするとオフにできます。

#### マップ
- ゲーム内マップに近い形の詳細マップ。探索済みの場所だけを見るか、全体を見るかを選べます。
- 残りの戦闘・キュリオ・トラップ・空腹マスの数と、キュリオに使う物資がいくつ必要かを表示します。
- マスにマウスを乗せると、敵の編成、キュリオに使う物資とその結果、トラップや障害物の効果、空腹が発生するかどうか、隠し部屋が分かります。
- 赤の宮廷の呪われた庭園のマップにも対応しています。

#### ルート案内・特殊エンカウント・明るさ
- クエスト用キュリオ、ボス、呪われた庭園までの**最短ルート**を案内します。
- シング・フロム・ザ・スターとファナティックはマップ上で**位置を示し**、コレクターとシャンブラーは**出現条件と確率**を表示します。
- 明るさによって変わるストレス・偵察・奇襲・回避・クリティカル・敵の命中とダメージ・追加ドロップの補正を**正確な数値**で表示します。

#### 戦闘
- このラウンドの味方と敵の**行動順**と、いま誰の番か。
- 肖像にマウスを乗せると**戦闘カード**が出ます。
  - 味方は、敵の各列を攻撃したときの命中・ダメージ・クリティカル・効果の確率。トリンケット・奇癖・病気・バフをすべて反映した最終値で、ゲームが表示しない隠し補正まで含めた実際の命中率です。
  - 敵は、味方の各列を攻撃したときの同じ数値に加えて、どのスキルを使うか・誰を狙うかの確率。
  - アボミネーションやデュエリストのようにモードが切り替わるキャラクターは、**現在のモード**の姿とスキルで表示します。
- **戦闘の引き延ばし（ストーリング）** — 次のラウンドに増援が来る危険度を色で示し、このラウンドに増援を防ぐ行動を何回したかをリアルタイムで数えます。
- **退却** — 成功確率と、行動順をオンにしていれば、いま退却したら成功するか失敗するか。
- **遠征メーター** — 中央のタイトルにマウスを乗せると、今回の遠征での英雄ごとの撃破数・与ダメージ・被ダメージ・HP回復・受けたストレス・ストレス回復・スタンを比較します。キャンプスキル・食事・アイテムでの回復も数えます。

#### アクティビティログ
- 戦闘と探索で起きたことを、ゲームの用語と色のまま記録します。スキル・命中・ダメージ・効果・抵抗・カウンター・心臓発作・勝手な行動から、キュリオ・トラップ・障害物・空腹まで。
- 判定は推測せず、**ゲームが表示した判定結果**をそのまま読み取って記録します。
- 戦闘が始まると自動でログに、終わるとマップに戻ります。
- ダンジョン1回につきログ1つ。セーブごとに直近10件を残すので、あとから見返せます。

#### 村
- ダンジョンと遠征の長さごとの**おすすめ物資数**。
- **データベース** — 敵・トリンケット・村のイベント・病気・徳・精神崩壊・奇癖を、どんな値からでも検索。
- **建物・区画の強化に必要な量** — 選んだ段階に必要な資源を、手持ち（領地＋遠征中に得た分）と比較します。効果の説明はゲーム内と同じで、遠征中にも開けます。

### インストール

1. [Releases](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest) から `AncestorsMap.zip` をダウンロードし、好きなフォルダに展開します。
2. `AncestorsMap.exe` を実行します。**.NET 8 Desktop Runtime** が必要で、入っていなければインストールの案内が表示されます。
3. ゲームを起動するとセーブを自動で見つけます。初めてなら **?** ボタンで画面ガイドを一度ご覧ください。

### 動作環境・互換性

- Windows 10/11、[.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0)。
- リアルタイムの情報（行動順・ストーリング・退却・キュリオの画面）を読むには、ゲームを **64ビットで起動**する必要があります。Steam の公開版と coming_in_hot ベータ、Steam 版・DRMフリー版（`_windowsnosteam`）の実行ファイルに対応しています。32ビット、またはまだ対応していないゲームのバージョンでは、メモリは読まず**セーブだけで動作**し、アクティビティログ上部のステータス欄に理由を表示します。
- MODは、セーブに記録された有効なMODの一覧と優先順位を読んで自動で反映します。ゲームデータを変更するほとんどのMODと一緒に使えます（ダンジョン追加MODは Farmstead Plus、The Sunward Isles、Vermintide で確認済み）。
- Steam 版をもとに作り、DRMフリー版の実行ファイルでも動作を確認しています。GOG など他のプラットフォームでは、ゲームやセーブの場所が異なり認識できない可能性があります。
- English・한국어・日本語・简体中文。最初はゲームの言語に合わせ、名前や説明はゲームの翻訳をそのまま使います（農場など、公式に訳されていない部分は日本語化MODの訳に従う場合があります）。

### 安全性

- セーブ・ゲームファイル・ゲームのメモリには**何も書き込みません**。ゲームにコードを差し込むこともありません（フック・インジェクションなし）。
- メモリは**読み取り専用**で開きます。セーブは1ターン遅れて書かれ、判定結果はセーブに残らないため、戦闘中の値をリアルタイムに合わせるためだけに使います。チートエンジンが値を探して**書き換える**のに対し、こちらは探して**表示する**だけです。
- 通信は**起動時の更新確認1回**（GitHub のリリース確認）だけです。アカウント・キー・データ収集はありません。
- 他のプログラムのメモリを読む性質上、一部のウイルス対策ソフトが誤検知することがあります。ダウンロードしたファイルが本物かどうかは、リリースノートの SHA-256 で確認できます。
- 画像や文章はインストール済みのゲームから読み込みます。ゲームの素材は同梱しておらず、アプリは実行ファイル1つ（約3.5MB）です。

### アップデート

新しいバージョンが出ると、アプリ起動時に案内が表示され、「更新を確認」を押すとこのリポジトリのリリースページが開きます。自動でダウンロードや置き換えはしません。新しい zip を受け取って上書きしてください。左上の署名をクリックすると、現在のバージョンと更新確認のボタンがあります。設定と遠征の記録は `%LocalAppData%\AncestorsMap` に残ります。

### 操作

| キー・マウス | 動作 |
|---|---|
| `` ` ``（Tab の上） | 表示・非表示 |
| `Caps Lock` | ゲームの**デフォルトの整列順**ボタンを押す（ゲームにショートカットのない機能） |
| `Home` | データベース・アクティビティログ・領地を閉じて基本画面（マップ）へ |
| 左ドラッグ・右ドラッグ | ウィンドウの移動・マップの移動 |
| ホイール・ホイールクリック | 拡大・縮小・マップとログの切り替え |
| ウィンドウの縁をドラッグ・上部のスライダー | ウィンドウの大きさ・透明度 |
| **?** ボタン・左上の署名 | 画面ガイド・アプリ情報（バージョン・更新確認） |

`` ` ``、`Caps Lock`、`Home`、ゲーム上でのホイールクリックは、**ゲーム画面が前面にあるときだけ**働き、他のプログラムでは通常どおり使えます。

### 既知の制限

- リアルタイムの情報は、対応している64ビット版のゲームでのみ読み取ります。ゲームがアップデートされると、アプリが新しいバージョンに対応するまではセーブだけで動作します。
- おすすめ物資の表は、英語版 Wiki・攻略記事・ダンジョン生成ルールの計算をまとめた参考値です。
- すべてのMODを検証できてはいません。おかしな表示があれば、下記からお知らせください。

### 不具合の報告

[Issues](https://github.com/Eolaloe/DD-AncestorsMap/issues) に、次の内容を添えて書いてください。
- アプリのバージョン（左上の署名をクリック）・ゲームのバージョン（Steam 公開版 / coming_in_hot / DRMフリー版）
- 有効にしているMODの一覧・どの画面で何をしたときか・できればスクリーンショット

### ライセンス・クレジット

[LICENSE](LICENSE) — 個人での利用は自由。再配布は改変せず出典を明記した場合のみ可。販売禁止。
Darkest Dungeon は Red Hook Studios のゲームです。このアプリはゲームの素材を含みません。
Claude と ChatGPT の助けを借りて作りました。

</details>

<details>
<summary><img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1e8-1f1f3.png" width="20" alt="🇨🇳"> <b>简体中文</b> — 《暗黑地牢》详细地图 · 战斗数据 · 活动日志悬浮窗</summary>

一款《暗黑地牢》悬浮窗工具，在游戏画面上方显示**游戏本身不会给你看的详细地牢地图、战斗数据和活动日志**。
即使游戏全屏也会始终置顶显示，点击工具窗口也不会抢走输入，操作仍然由游戏接收。

工具里没有写死任何原版数据。它会**读取当前存档所启用的本体、DLC 和所有模组的数据并合并**，因此模组新增或修改的奇物、敌人、饰品和特质，也会按游戏内的实际数值显示。读取另一个存档时会自动重新同步。

### 功能一览

- **详细地图** — 与游戏内地图同样的布局。鼠标悬停在格子上即可查看奇物、陷阱、敌人编组和互动结果。提供前往任务奇物、首领和庭院的**最短路线导航**、尚未互动奇物所需的**补给追踪**、侦察几率、亮度带来的修正数值，以及特殊遭遇（星空怪、狂信者、跛行者、收集者）的提示。
- **战斗信息** — 每个站位可用技能的命中、伤害、暴击和效果几率，敌人可能对谁使用哪个技能，行动顺序，拖回合（Stalling）计数（本回合做了几次阻止增援的行动、下回合会发生什么），以及撤退判定。
- **活动日志与统计** — 自动记录战斗、探索和扎营，并以柱状图比较每位英雄的击杀、造成伤害、承受伤害、治疗和压力。
- **数据库搜索** — 敌人、饰品、城镇事件、疾病、美德、折磨和特质，可按名称、稀有度、职业、效果等任意值搜索，模组内容也包括在内。
- **在小镇时** — 按地牢和远征长度给出**推荐补给**，并计算建筑和区域建筑升级**所需资源**（与现有资源加本次远征所得相比较）。
- **界面引导** — 点击右上角的 **?** 按钮，会逐步讲解每个界面（使用示例远征，在小镇里也能看）。

部分功能会显示游戏刻意隐藏的信息。地图默认**只显示已探索的区域**，全图显示可通过顶部按钮切换。行动顺序和撤退成败默认开启，点击战斗栏中间的标题即可关闭。

#### 地图
- 与游戏内地图相近的详细地图，可选择只看已探索区域或查看整张地图。
- 显示剩余的战斗、奇物、陷阱和饥饿格数量，以及奇物需要多少补给。
- 鼠标悬停在格子上可查看敌人编组、奇物所需的补给及结果、陷阱和障碍的效果、是否即将触发饥饿，以及隐藏房间。
- 支持猩红庭院 DLC 的庭院地图。

#### 路线导航、特殊遭遇、亮度
- 为任务奇物、首领和庭院导航**最短路线**。
- 星空怪和狂信者会在地图上**标出位置**，收集者和跛行者则显示**出现条件和几率**。
- 以**精确数值**显示亮度对压力、侦察、偷袭、闪避、暴击、敌人命中与伤害、额外战利品的影响。

#### 战斗
- 本回合敌我双方的**行动顺序**，以及当前轮到谁。
- 鼠标悬停在头像上会弹出**战斗卡片**。
  - 我方：攻击敌方每一列时的命中、伤害、暴击和效果几率。这是计入饰品、特质、疾病和增益后的最终数值，并包含游戏不会显示的隐藏修正，是真实的命中率。
  - 敌方：攻击我方每一列时的同类数值，以及会使用哪个技能、会瞄准谁的几率。
  - 憎恶、决斗者这类会切换形态的角色，会按**当前形态**的外观和技能显示。
- **拖回合（Stalling）** — 用颜色提示下回合出现增援的风险，并实时统计本回合做了几次阻止增援的行动。
- **撤退** — 显示成功几率；开启行动顺序时，还会告诉你现在撤退是成功还是失败。
- **远征统计** — 鼠标悬停在中间的标题上，可比较本次远征中每位英雄的击杀、造成伤害、承受伤害、生命恢复、承受压力、压力缓解和眩晕次数。扎营技能、进食和道具治疗也会计入。

#### 活动日志
- 用游戏本身的用语和颜色记录战斗与探索中发生的一切：技能、命中、伤害、效果、抵抗、反击、心脏病发作、擅自行动，以及奇物、陷阱、障碍和饥饿。
- 判定结果不靠推测，而是直接读取**游戏显示的判定结果**。
- 战斗开始时自动切换到日志，结束后回到地图。
- 每次进入地牢生成一份日志，每个存档保留最近 10 份，方便回顾。

#### 小镇
- 每个地牢和远征长度的**推荐补给数量**。
- **数据库** — 敌人、饰品、城镇事件、疾病、美德、折磨和特质，可按任意值搜索。
- **建筑与区域建筑所需资源** — 将所选升级阶段的需求与现有资源（领地加远征中获得的部分）进行比较。效果说明与游戏内一致，远征途中也能打开。

### 安装

1. 从 [Releases](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest) 下载 `AncestorsMap.zip`，解压到任意文件夹。
2. 运行 `AncestorsMap.exe`。需要 **.NET 8 Desktop Runtime**，如果没有安装，会弹出安装提示。
3. 启动游戏后会自动找到存档。第一次使用时，建议点 **?** 按钮看一遍界面引导。

### 运行环境与兼容性

- Windows 10/11，[.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0)。
- 要读取实时数据（行动顺序、拖回合、撤退、奇物互动窗口），游戏必须以 **64 位运行**。支持 Steam 正式版和 coming_in_hot 测试版，Steam 版与无 DRM 版（`_windowsnosteam`）的可执行文件均可。如果是 32 位或尚未适配的游戏版本，工具不会读取内存，**只依靠存档运行**，并在活动日志上方的状态栏说明原因。
- 模组会根据存档中记录的启用列表和加载顺序自动生效。可与大多数修改游戏数据的模组一起使用（新增地牢的模组已在 Farmstead Plus、The Sunward Isles、Vermintide 上验证）。
- 基于 Steam 版开发和测试，也确认可在无 DRM 版可执行文件上运行。GOG 等其他平台的游戏或存档位置可能不同，可能无法识别。
- English · 한국어 · 日本語 · 简体中文。默认跟随游戏语言，名称和说明直接使用游戏的翻译。

### 安全性

- **不会写入**存档、游戏文件或游戏内存，也不会向游戏注入任何代码（无挂钩、无注入）。
- 游戏内存以**只读**方式打开。存档会晚一回合写入，判定结果也不会保存在存档里，因此内存只用于让战斗数据保持实时。CE 修改器是找到数值后**修改**它，而本工具只是找到数值后**显示**出来。
- 唯一的网络通信是**启动时的一次更新检查**（查询 GitHub 发布页）。不需要账号或密钥，也不收集任何数据。
- 由于会读取其他程序的内存，部分杀毒软件可能会误报。可以用发布说明中的 SHA-256 核对下载的文件是否为原版。
- 图片和文字均从已安装的游戏中读取，不附带任何游戏素材，工具本身只是一个约 3.5 MB 的可执行文件。

### 更新

有新版本时，启动工具会弹出提示，点击「检查更新」会打开本仓库的发布页面。不会自动下载或替换，下载新的 zip 覆盖即可。点击左上角的署名，可以查看当前版本并检查更新。设置和远征记录保存在 `%LocalAppData%\AncestorsMap`。

### 操作

| 按键 / 鼠标 | 功能 |
|---|---|
| `` ` ``（Tab 键上方） | 显示 / 隐藏 |
| `Caps Lock` | 按下游戏中的**初始队伍阵型**按钮（游戏没有为此提供快捷键） |
| `Home` | 关闭数据库、活动日志或领地界面，回到默认界面（地图） |
| 左键拖动 · 右键拖动 | 移动窗口 · 移动地图 |
| 滚轮 · 滚轮点击 | 缩放 · 在地图和日志之间切换 |
| 拖动窗口边缘 · 顶部滑块 | 调整窗口大小 · 透明度 |
| **?** 按钮 · 左上角署名 | 界面引导 · 工具信息（版本、检查更新） |

`` ` ``、`Caps Lock`、`Home` 以及在游戏上的滚轮点击，**只在游戏窗口位于前台时生效**，在其他程序中照常使用。

### 已知限制

- 实时数据只在已适配的 64 位游戏版本上读取。游戏更新后，在工具适配新版本之前只依靠存档运行。
- 推荐补给表综合了英文 Wiki、社区攻略和地牢生成规则的计算，仅供参考。
- 并未验证所有模组。如果显示有异常，欢迎通过下方渠道反馈。

### 问题反馈

请在 [Issues](https://github.com/Eolaloe/DD-AncestorsMap/issues) 中附上以下信息：
- 工具版本（点击左上角署名）和游戏版本（Steam 正式版 / coming_in_hot / 无 DRM 版）
- 已启用的模组列表、在哪个界面做了什么操作，最好附上截图

### 许可与致谢

[LICENSE](LICENSE) — 可自由用于个人用途；仅允许在不做修改并注明出处的情况下再分发；禁止售卖。
《暗黑地牢》（Darkest Dungeon）是 Red Hook Studios 的游戏，本工具不包含任何游戏素材。
在 Claude 和 ChatGPT 的协助下制作。

</details>

---

<img src="https://github.githubassets.com/images/icons/emoji/unicode/1f1fa-1f1f8.png" width="20" alt="🇺🇸"> <b>English</b>

An overlay for Darkest Dungeon that puts **the dungeon map, combat numbers and an activity log the game never shows you** right on top of your game.
It stays on top even over a fullscreen game, and clicking it doesn't steal your input — the game keeps receiving it.

Nothing is hard-coded from vanilla. It **reads the base game, DLC and every mod enabled in your current save and merges them**, so curios, monsters, trinkets and quirks added or changed by mods show up with their real in-game values. Load a different save and it re-syncs on its own.

## What it does

- **Detailed map** — Laid out like the in-game map. Hover any tile for curios, traps, enemy groups and interaction results. **Shortest-route guidance** to quest curios, the boss and the Courtyard, a **provision tracker** for curios you haven't touched yet, scouting chance, exact light-level modifiers, and alerts for special encounters (Thing from the Stars, Fanatic, Shambler, Collector).
- **Combat info** — Accuracy, damage, crit and effect chance for every skill from every rank, which skill an enemy is likely to use and on whom, turn order, a stalling tracker (how many anti-reinforcement actions you've taken this round and what the next round will bring), and retreat odds.
- **Activity log & meter** — Combat, exploration and camping are logged automatically, and a meter compares each hero's kills, damage dealt and taken, healing and stress.
- **Database search** — Look up enemies, trinkets, town events, diseases, virtues, afflictions and quirks by name, rarity, class or effect. Modded entries included.
- **In the Hamlet** — **Recommended provisions** by dungeon and length, and a **cost calculator** for building and district upgrades (against what you own plus this expedition's haul).
- **Guided tour** — Press the **?** button in the top-right corner for a step-by-step tour of each screen (it uses a sample expedition, so it works in town too).

Some features reveal information the game deliberately hides. By default the map shows **only explored areas**; the full map is a toggle at the top. Turn order and the retreat outcome are on by default — click the title in the middle of the combat bar to turn them off.

<details>
<summary>Full feature list</summary>

### Map
- A detailed map shaped like the in-game one. Choose between explored areas only and the whole dungeon.
- Counts of remaining battles, curios, traps and hunger tiles, plus how many provisions your curios will need.
- Hover a tile to see the enemy group, which provisions a curio takes and what they do, trap and obstacle effects, whether hunger is about to hit, and secret rooms.
- Supports the Crimson Court's Courtyard maps.

### Routing, special encounters, light
- The **shortest route** to quest curios, the boss and the Courtyard.
- **Pinpoints** the Thing from the Stars and the Fanatic on the map, and shows **trigger conditions and odds** for the Collector and the Shambler.
- **Exact numbers** for every light-level effect: stress, scouting, surprise, dodge, crit, enemy accuracy and damage, and bonus loot.

### Combat
- This round's **turn order** for both sides, and whose turn it is right now.
- Hover a portrait for a **combat card**.
  - For heroes: accuracy, damage, crit and effect chance against each enemy rank — final values with trinkets, quirks, diseases and buffs applied, including hidden modifiers the game never displays.
  - For enemies: the same numbers against each hero rank, plus the odds of which skill they'll use and who they'll target.
  - Characters that change modes, like the Abomination or the Duelist, are shown in **their current mode** with that mode's skills.
- **Stalling** — Color-coded risk of reinforcements next round, and a live count of anti-reinforcement actions taken this round.
- **Retreat** — Success chance, and with turn order enabled, whether retreating right now will succeed.
- **Expedition meter** — Hover the title in the middle to compare each hero's kills, damage dealt, damage taken, HP healed, stress taken, stress healed and stuns this expedition. Camping skills, meals and item heals count too.

### Activity log
- Records everything that happens in combat and exploration, using the game's own wording and colors: skills, hits, damage, effects, resists, ripostes, heart attacks and act-outs, plus curios, traps, obstacles and hunger.
- Outcomes aren't guessed — it reads **the results the game itself displays**.
- Switches to the log when a battle starts and back to the map when it ends.
- One log per dungeon run; the last 10 per save are kept so you can look back.

### Hamlet
- **Recommended provision counts** for each dungeon and expedition length.
- **Database** — Search enemies, trinkets, town events, diseases, virtues, afflictions and quirks by any value.
- **Building & district costs** — Compares what a chosen upgrade tier needs against what you have (estate plus this expedition's loot). Effect text matches the game, and it's available mid-expedition too.

</details>

## Installation

1. Download `AncestorsMap.zip` from [Releases](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest) and extract it anywhere.
2. Run `AncestorsMap.exe`. It needs the **.NET 8 Desktop Runtime** — if it's missing, Windows will point you to the installer.
3. Launch the game and the app finds your save automatically. On first run, take the tour with the **?** button.

## Requirements & compatibility

- Windows 10/11 and the [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0).
- Live combat data (turn order, stalling, retreat, curio windows) requires running the game **as 64-bit**. Supported: the Steam public build and the coming_in_hot beta, with either the Steam or the DRM-free (`_windowsnosteam`) executable. On 32-bit or an unrecognized game version the app skips memory reading, **runs from your save alone**, and tells you why in the status line above the activity log.
- Mods are picked up automatically from the enabled list and load order in your save. Works alongside most mods that change game data (dungeon mods tested: Farmstead Plus, The Sunward Isles, Vermintide).
- Built and tested on the Steam version, and confirmed on the DRM-free executable. Other platforms such as GOG may store the game or saves elsewhere and might not be detected.
- English · 한국어 · 日本語 · 简体中文. It follows the game's language at first and uses the game's own translations for names and descriptions.

## Safety

- It **never writes** to your saves, game files or game memory, and never injects anything into the game (no hooks, no injection).
- Game memory is opened **read-only**. Saves are written a turn late and roll outcomes aren't saved at all, so memory is used only to keep combat info live. Unlike Cheat Engine, which finds values to **change** them, this only finds values to **show** them.
- The only network traffic is **one update check at startup** (a GitHub release lookup). No accounts, no keys, no data collection.
- Because it reads another program's memory, some antivirus software may flag it. You can verify your download against the SHA-256 in the release notes.
- Art and text are read from your game install. No game assets are bundled — the app is a single ~3.5 MB executable.

## Updates

When a new version is out, a notice appears when you start the app, and **Check for updates** opens this repository's release page. Nothing is downloaded or replaced automatically — just grab the new zip and overwrite. Click the signature in the top-left corner to see your current version and check for updates. Settings and expedition logs are kept in `%LocalAppData%\AncestorsMap`.

## Controls

| Key / mouse | Action |
|---|---|
| `` ` `` (above Tab) | Show / hide |
| `Caps Lock` | Presses the game's **Default Party Order** button (the game has no hotkey for it) |
| `Home` | Close the database, log or estate view and return to the map |
| Left-drag · right-drag | Move the window · pan the map |
| Wheel · wheel click | Zoom · switch between map and log |
| Drag window edge · top slider | Resize · opacity |
| **?** button · top-left signature | Guided tour · app info (version, update check) |

`` ` ``, `Caps Lock`, `Home` and wheel-clicking over the game **only work while the game window is in front**; everywhere else they behave normally.

## Known limitations

- Live data is only read on supported 64-bit game versions. After a game update, the app runs from saves alone until it's updated for the new version.
- The recommended provisions table combines the English wiki, community guides and the dungeon generation rules — treat it as a guide.
- Not every mod has been tested. If something looks off, please report it below.

## Reporting issues

Open an [issue](https://github.com/Eolaloe/DD-AncestorsMap/issues) and include:
- App version (click the signature, top left) and game version (Steam public / coming_in_hot / DRM-free)
- Your enabled mods, which screen you were on and what you did, and a screenshot if you can

## License & credits

[LICENSE](LICENSE) — free for personal use; redistribution only unmodified and with attribution; no selling.
Darkest Dungeon is a game by Red Hook Studios. This app doesn't include any game assets.
Made with help from Claude and ChatGPT.
