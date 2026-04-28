# 画像制作ブリーフ — career-school LP

LP内のすべての画像プレースホルダーは仮の枠で表示されています。本制作前に下記スペックで画像を用意・差し替えてください。

## トーン共通仕様

- **色味**: 暖色寄り（ピンク〜オレンジ〜淡いイエロー）。背景は明るく抜け感のある自然光。
- **モデル**: 20代後半〜30代前半の女性中心。多様な年齢層・体型・髪型を意識し、ステレオタイプ回避。
- **表情**: 過度な笑顔ではなく、穏やかで前向きな自然な表情。
- **ロケーション**: カフェ・自宅リビング・ワークスペースなど「ライフスタイル感」のある場所。スタジオ撮りは避ける。
- **画質**: WebPメイン（JPG/PNG fallback）/ Retina 2x想定（2400px長辺）

---

## #FV01 — ヒーローメインビジュアル
| 項目 | 仕様 |
|---|---|
| サイズ | 1200×1500px（4:5縦長） |
| 内容 | 20代後半女性がノートPCを開いて軽やかに作業しているシーン |
| 背景 | カフェ or 自宅。窓辺の自然光・観葉植物・カップ |
| 雰囲気 | 「私もこれならできそう」と思わせる等身大の余裕感 |
| NG | 過剰なドヤ顔・スーツ・オフィス感・男性の登場 |

## #BNF01 #BNF02 #BNF03 — 3つの理由 アイコン
| ID | 内容 |
|---|---|
| #BNF01 | 「複数スキル」を象徴するイラストアイコン（ノートPC + ペン + カメラがオーバーラップ） |
| #BNF02 | 女性同士のオンラインコーチング画面（ZoomUI風の縦並びサムネ） |
| #BNF03 | 受講生コミュニティの集合感（女性4-6人の小さな円形アバターを輪状に配置） |

各 480×480px / フラット系イラスト or 写真切り抜き合成

## #SKL01〜#SKL08 — スキルカード画像
| ID | スキル | ビジュアル要素 |
|---|---|---|
| #SKL01 | Webデザイン | Figma画面 + カラーパレット |
| #SKL02 | ライティング | 原稿用紙 or タイピング手元 + コーヒー |
| #SKL03 | 動画編集 | タイムライン編集画面の一部 |
| #SKL04 | SNSマーケ | 分析ダッシュボードの一部 |
| #SKL05 | イラスト/写真 | ペンタブ + ミラーレスカメラ |
| #SKL06 | プログラミング | コードエディタの画面 |
| #SKL07 | コーチング | 1on1対話シーンのシルエット |
| #SKL08 | その他 | 各種ツールアイコンのコラージュ |

各 600×600px / 統一感ある合成・トーン揃え

## #VOC01〜#VOC04 — 受講生顔写真
| ID | プロフィール | 雰囲気 |
|---|---|---|
| #VOC01 | 28歳女性・元事務職 | カジュアル・笑顔バストショット |
| #VOC02 | 32歳女性・育休中 | 子供との自然なシーン（顔バレない範囲） |
| #VOC03 | 35歳女性・営業職 | カフェで作業する横顔・スマートカジュアル |
| #VOC04 | 27歳女性・派遣社員 → 正社員 | パートナーと一緒の写真・親しみやすい |

各 400×400px 円形トリミング想定

⚠️ **重要**: 実在する受講生の顔写真を使う場合は必ず本人同意・モデルリリース取得。
ストック写真の場合は「お客様の声」とは別に「※イメージ」表記推奨（景表法対策）。

## #PRZ01〜#PRZ03 — キャンペーンプレゼント画像（Wチャンス訴求）

LP最下部のキャンペーンセクションで使用する商品ビジュアル。商品が一目で分かることを最優先しつつ、LP全体のトーン（暖色寄り・ピンク〜ピーチ）と調和させる。

| 項目 | 仕様 |
|---|---|
| サイズ | 1200×900px（4:3横長） |
| 背景 | 淡いピーチ／クリーム（#FFE9DE〜#FFF3EC）の単色 or 緩やかなグラデ |
| ライティング | 柔らかいトップライト・自然な影 |
| 構図 | 中央配置、上下左右に約15%の余白（CSSで `qty` バッジを右上に重ねるため） |
| トーン | エディトリアル系商品写真、過度な広告感を避ける |
| 共通NG | ロゴ・ブランド名の強調、派手なキャッチコピー、ステッカー等の合成 |

### #PRZ01 — ハワイ旅行
ファイル名: `prize-hawaii.png`
ビジュアル: 白砂のビーチ、ヤシの葉、海の青、太陽光の煌めき。ライフスタイル感のある旅行イメージ（人物は入れない or シルエット程度）。

```
A bright dreamy Hawaiian beach scene from a low angle, soft turquoise ocean waves, 
white sand, gentle palm leaves framing the corners, golden afternoon sunlight, 
peach-pink sky in the upper background, editorial travel photography style, 
warm cinematic color grading, no people, no text, clean composition with 
generous negative space in the upper-right area, 4:3 horizontal,
soft pastel mood matching coral and cream interior brand palette
```

### #PRZ02 — MacBook Pro
ファイル名: `prize-macbook.png`
ビジュアル: シルバーの13–14インチMacBook Proを斜め45度の俯瞰で撮影。画面はOFF or 淡いデスクトップ。机上は無地のテーブル＋小物（コーヒーカップ等は不要、シンプルに）。

```
A modern silver laptop computer (slim aluminum unibody, no visible logos) 
shown at a slight 30-degree top-down angle, lid open at 110 degrees, 
screen showing a soft pastel desktop, sitting on a smooth peach-cream surface, 
soft directional studio lighting from upper left, gentle realistic shadow, 
editorial product photography, minimal composition, 4:3 horizontal frame, 
generous negative space, warm color palette matching coral/peach brand tone, 
no text, no brand logos, no other objects in frame
```

### #PRZ03 — iPad & Apple Pencil
ファイル名: `prize-ipad.png`
ビジュアル: タブレット端末（iPad様）+ スタイラスペンを並列配置。タブレット画面にはイラスト or デザイン作業のモック。LPユーザー（クリエイター志向の女性）にとっての"なりたい姿"を象徴。

```
A sleek modern tablet computer with a stylus pen placed diagonally beside it, 
top-down flat lay composition, tablet screen displaying a soft sketch or 
gentle pastel illustration in progress, peach-cream background surface, 
soft natural lighting from upper right, subtle realistic shadow, 
editorial flat lay photography style, minimal warm color palette 
(coral, peach, cream), 4:3 horizontal aspect ratio, generous negative space, 
no text, no visible brand logos, lifestyle-creative mood
```

### 配置先

| ID | LP内 data-prize-id | 表示位置 |
|---|---|---|
| #PRZ01 | `hawaii` | 「申し込みで」グループ・上段 |
| #PRZ02 | `macbook` | 「申し込みで」グループ・下段 |
| #PRZ03 | `ipad` | 「さらに参加で」グループ |

⚠️ **景表法注意**: 実際のキャンペーンで配布する商品と画像が大きく異なる場合は誤認を招くため、必ず現物に近いビジュアルを用意するか「※イメージ」表記を併記すること。

---

## 補足：画像生成AIで仮制作する場合のプロンプト例

```
A young Japanese woman in her late 20s working on a laptop in a sunlit cafe,
warm pink and orange tones, soft natural lighting, casual and approachable
expression, lifestyle photography style, vertical 4:5 composition, 
bokeh background with plants
```

各画像のスタイルガイドが揃ったら、Midjourney / Nano Banana / Adobe Firefly等で仮ビジュアルを起こし、本撮影のキービジュアル設計に活かしてください。
