# 生成プロンプト集 — ImageFX (Imagen 3) / FLOW (Veo 3)

> **主力ペルソナ：中村早紀（29歳・法人営業・営業辞めずに副業から月+5万）**
> ペルソナ表の「暮らし美学系・ドキュメンタリー風・直球の煽り回避」を全プロンプトで徹底。

---

## 素材総数

| 区分 | 数 | 用途 |
|---|---|---|
| 画像 | **17** | FV3 + 共感2 + ストーリー4 + ベネフィット3 + スキル8 + 顔4 + CTA1 |
| 動画 | **4** | FV直下ループ + モンタージュ + 1on1 + 画面操作 |
| **合計** | **21素材** | |

**追加でA/Bテスト・差し替え用に画像10〜15枚あると安全**（合計27〜32点）。

---

## ImageFX プロンプトの基本ルール

ImageFX (Google Imagen 3) は **自然言語の短めの描写** を好みます。

- 50〜80語程度がベスト（長すぎると要素を取りこぼす）
- アスペクト比は **UIで選択**（Portrait / Square / Landscape / Widescreen）
- ネガティブプロンプトはないので、避けたい要素は省略する設計
- スタイル・カメラ・光は文末にコンマ区切りで追加すると効きやすい
- 「Japanese woman」など人種を明示しないとアジア系混合になりがち

## FLOW (Veo 3) プロンプトの基本ルール

- 8秒上限（FLOW標準）
- アスペクト比は 16:9 / 9:16 から選択（UI）
- 動画なので **動詞・カメラ移動・音**を入れる
- 「Audio:」で環境音を指定可能（Veo 3は音も生成）
- ループ用には "seamless loop" / "ends in same position as start" と明記

---

# A. FV — ファーストビュー（3案 / A/Bテスト）

## A-01 「カフェの昼休み」

**シーン**: 営業の昼休み・近所のカフェで、スマホで動画講座を見ながらメモを取る  
**アスペクト**: Portrait 4:5 (ImageFXで「Portrait」選択)

```
A Japanese woman in her late 20s sits alone at a quiet neighborhood
cafe in Tokyo during lunch break. She holds a smartphone showing
a learning video, a small open notebook and a pen on the wooden
table beside a half-empty oat milk latte. She wears a beige knit
cardigan over a white linen shirt, soft no-makeup makeup, hair in
a low ponytail. Contemplative yet hopeful expression, gaze on the
phone. Soft afternoon window light, slightly desaturated warm tones.
Documentary lifestyle photography, 35mm prime lens look, shallow
depth of field, cinematic film grain.
```

## A-02 「自宅の夜・ノートPC」

**シーン**: 終電帰りの自宅で、ノートPC前にハーブティーと小さな成功感  
**アスペクト**: Portrait 4:5

```
A Japanese woman in her late 20s sits at a wooden desk by a
window in a small modern Tokyo apartment late at night. A 13-inch
silver laptop is open in front of her, soft warm lamp light from
a single floor lamp, a steaming cup of herbal tea beside her, a
small plant and stacked books in the background. She wears an
oversized cream sweatshirt, glasses, hair tied up loosely. Half
of her face lit by warm lamp light, focused calm expression with
a small private smile. Cozy domestic scene, lifestyle documentary,
35mm look, warm desaturated palette, plenty of negative space.
```

## A-03 「土曜の朝・サウナ後」

**シーン**: サウナの帰り道、北欧風カフェで自分の時間  
**アスペクト**: Portrait 4:5

```
Saturday morning, a Japanese woman in her late 20s sits at a
Scandinavian-style cafe counter facing a window in Tokyo, holding
a hot drink with both hands. Fresh face after a sauna session,
hair slightly damp, no makeup. She wears a relaxed cream pullover.
Soft golden hour light streams in, her face glowing with calm.
Looking out the window with a thoughtful half-smile. Uncrowded
cafe, plants, wood textures. Documentary lifestyle photography,
35mm look, warm soft palette, dreamy slightly grainy film aesthetic.
```

---

# B. 共感セクション

## B-01 「終電後の駅で立ち止まる」

**アスペクト**: Portrait 4:5

```
A Japanese businesswoman in her late 20s wearing a navy blazer
over a white blouse, holding a tote bag, stands on an empty
suburban Tokyo train platform at night. Neon signs glow softly
in the distance. She looks down at her phone with a tired
contemplative expression, slightly furrowed brow. Cinematic
documentary photo, 35mm look, cool but warm-tinted lighting,
slight motion blur in the background of a passing train.
```

## B-02 「会議後・自分の評価シートを見る」

**アスペクト**: Landscape 16:9

```
Over-the-shoulder close-up shot of a Japanese woman in her late
20s at her office desk in late afternoon, looking down at a
printed career evaluation sheet on the desk, a half-empty coffee
cup beside it. Soft window light from the side. Her face partially
visible in profile, subtle frown, slight head tilt. Realistic
office environment with blurred coworkers in background. Documentary
photo, 35mm, slightly desaturated warm tones.
```

---

# C. ストーリー4カット（同一モデルで連続性）

> **重要**: C-01 〜 C-04 と F-01 と A-01 は **同じ人物の連続ドキュメンタリー** に見せる。
> ImageFXの場合、最初の1枚を作ってから「Add to canvas」で同モデルの差分を作るとベター。

## C-01 「9月・申込んだ夜」

**アスペクト**: Landscape 16:9

```
Inside a small Tokyo studio apartment at night, soft warm lamp
light only. A Japanese woman in her late 20s sits cross-legged
on a beige sofa with a thin blanket, a tablet propped on a side
table showing a video orientation. She wears cream loungewear,
hair in a messy bun, holds a notebook. Face lit by the screen,
attentive nervous-but-excited expression. Tea cup nearby, soft
plants in corner. Cinematic intimate scene, lifestyle documentary,
35mm look, warm low-light palette.
```

## C-02 「12月・課題提出の夜」

**アスペクト**: Landscape 16:9

```
The same Japanese woman in her late 20s, three months later, with
slightly more confident posture. She sits at a small desk in her
Tokyo apartment late at night, just clicked submit on her laptop,
a small victorious smile, leaning back with both hands behind her
head. Course notes around her, sticky notes on the wall in blurred
background showing weekly schedule, a half-eaten onigiri, tea.
Soft warm lamp light, single light source, cozy. Documentary photo,
35mm, warm tones.
```

## C-03 「2月・初案件の打ち合わせ」

**アスペクト**: Landscape 16:9

```
The same Japanese woman in her late 20s, now in winter daytime
at a chic neighborhood cafe in central Tokyo. She wears a soft
camel turtleneck and a delicate gold necklace, sits across from
a client (out of frame), her laptop open showing a simple Figma
design mockup. Mid-conversation, confident relaxed smile, both
hands gesturing slightly. Natural window light, warm wood interior,
plants. Documentary candid feel, 35mm, slight film grain, warm
desaturated palette.
```

## C-04 「3月・振込通知を見る朝」

**アスペクト**: Landscape 16:9

```
Sunday morning in a small but tasteful Tokyo apartment. The same
Japanese woman in her late 20s in cream pajamas sits on her bed
with morning sunlight pouring through sheer curtains. She holds
her smartphone showing a bank notification (numbers blurred).
Soft surprised-then-smiling expression, hand half covering her
mouth, not exaggerated. Coffee cup on bedside table, beige and
cream bedding. Domestic intimate documentary photo, 35mm look,
golden hour light, warm hues.
```

---

# D. ベネフィット 3 連バナー

## D-01 「40+のスキル」を象徴する静物

**アスペクト**: Widescreen 16:9（ImageFX UIで Widescreen 選択）

```
Editorial top-down still life photography. A clean cream-beige
tabletop, an open silver laptop in the center showing a soft
abstract learning dashboard mockup. Around it: a Wacom-style pen
tablet, a small mirrorless camera, a sketch pad with simple line
drawings, colorful Post-it notes in muted pastels, a coffee cup,
a smartphone showing a simple analytics graph, a small plant.
Warm natural light from upper left, generous negative space on
the right. No people, no real brand logos.
```

## D-02 「専属コーチング」を象徴

**アスペクト**: Widescreen 16:9

```
Wide horizontal frame, split composition. On the left, a Japanese
woman in her late 20s on a video call on her laptop, slight side
angle, soft smile, casual home setting with a plant. On the right,
a Japanese woman in her early 30s on the other side of the call,
in a different home or office environment, taking notes, warm
engaged expression. Both sides share warm beige aesthetic. Window
light, lifestyle documentary, 35mm look. Slight blur to suggest
connection between the two scenes.
```

## D-03 「コミュニティ・仲間と学ぶ」

**アスペクト**: Widescreen 16:9

```
Wide horizontal banner. A small offline meetup of five Japanese
women in their late 20s to early 30s, casually seated around a
low table at a beautiful neighborhood cafe in Tokyo. Laptops and
notebooks open, mid-conversation, some laughing softly, some
pointing at a screen. Diverse hairstyles and casual fashion,
warm wood interior, plants, window natural light. Documentary
candid photo, 35mm look, soft warm desaturated tones, slight film
grain. No men, no school uniform vibe.
```

---

# E. スキルカード（無人静物・正方形）

> **共通テンプレート**: 全8枚を同じ撮影セット感で揃える。配色：cream / beige / terracotta / sage。

## E-01 Webマーケ

```
Top-down editorial still life. A slim silver laptop on a beige
desk shows a clean abstract analytics dashboard with simple line
graphs and bar charts (no real logos). A coffee cup, a notebook
with handwritten notes, a small plant. Soft window natural light,
warm desaturated palette. No people. Square composition.
```

## E-02 Webデザイン

```
Top-down editorial still life. A tablet on a beige desk displays
a soft pastel design mockup. Beside it: a Wacom pen, color swatch
cards in beige/terracotta/sage, a small sketchbook with pencil
sketches. Window natural light. Warm tones. No people. Square.
```

## E-03 SNS運用

```
Top-down still life. A smartphone on a cream desk shows an
abstract Instagram-like grid (no real handles). Beside: a notebook
with content calendar handwritten, a coffee cup, dried flowers.
Warm natural light. Editorial flat-lay. Square composition.
```

## E-04 ライティング

```
Close-up editorial flat-lay. An open notebook with handwritten
abstract notes (not legible specific text), a fountain pen, a
steaming coffee cup, a slim laptop slightly open in the corner.
Beige desk, warm window light. Square composition.
```

## E-05 動画編集

```
Top-down still life. A laptop showing a simple abstract video
editing timeline (vague), a wired headphone, a small notebook,
a coffee. Beige desk, warm light. Editorial flat-lay. Square.
```

## E-06 カメラ・写真

```
Top-down still life. A mirrorless camera body (no logos visible)
on a beige desk, beside a beige notebook, a few printed photos
of nature, a small plant. Warm natural light. Editorial. Square.
```

## E-07 イラスト

```
Top-down close-up. A tablet with a digital pen, mid-illustration
of a simple line-art portrait. Color palette of beige and
terracotta cards beside it. Warm desk, natural light. Square.
```

## E-08 その他

```
Soft editorial collage. Stacked books, a pencil, a coffee cup,
a small plant, a smartphone, blurred and overlapping in a warm
beige palette. Dreamy editorial still life. Square composition.
```

---

# F. 受講生顔写真（4ペルソナ・正方形）

## F-01 中村早紀像（元法人営業 → Webマーケ副業）

```
Portrait of a Japanese woman in her late 20s, soft natural makeup,
warm gentle smile, wearing a beige knit. Sitting at a softly lit
cafe with blurred bokeh background. Documentary lifestyle photo,
35mm look, warm tones. Square composition.
```

## F-02 木村ほのか像（元一般事務 → SNS運用副業）

```
Portrait of a Japanese woman around 27, slightly shy warm smile,
hair in soft layers, wearing a cream blouse. Sitting near a window
in a casual home setting, plants in blurred background. Lifestyle
photo, 35mm. Square.
```

## F-03 渡辺莉子像（元アパレル販売 → Webデザイン）

```
Portrait of a stylish Japanese woman around 31, expressive eyes,
soft side smile, wearing a camel turtleneck and statement earrings.
Sitting at a chic cafe with warm wood interior in blurred
background. 35mm documentary photo, warm tones. Square.
```

## F-04 林真央像（元病棟看護師 → 医療ライター副業）

```
Portrait of a calm Japanese woman around 33, warm steady smile,
wearing a soft cream cardigan. Sitting at a desk in a tidy living
room with morning natural light, blurred shelves with books in
background. 35mm lifestyle photo. Square.
```

---

# G. CTA帯バナー

## G-01 「無料説明会」誘導用

**アスペクト**: Widescreen 16:9（クロップして帯状に使う）

```
Wide horizontal scene, soft blurred background of a Tokyo cafe
or home workspace with warm natural light, beige and cream tones.
A faint silhouette of a woman holding a smartphone in the lower
right third. Mostly atmospheric negative space for a button to
be overlaid in CSS. No people fully visible. Editorial lifestyle
photo, slight film grain. Warm desaturated.
```

---

# V. 動画素材（4本・FLOW / Veo 3）

> **共通仕様**: 8秒前後・無音または環境音のみ・seamless loop推奨・16:9

## V-01 FV直下「カフェでメモを取る手元」

```
A close-up cinematic shot. Top-down view of a young Japanese
woman's hand holding a pen, writing soft handwritten notes in a
beige notebook on a cafe table. Beside the notebook, a smartphone
is propped showing a video lecture (vague content, no logos). A
cup of latte half visible. Warm natural window light, soft cream
and beige palette, slight film grain. Camera completely static.
The hand pauses, considers, then writes a small underline. Loops
seamlessly back to start position.

Audio: ambient cafe — gentle espresso machine in distance, faint
soft jazz, no voices.

Duration: 8 seconds. Aspect: 16:9.
```

## V-02 「半年で変わる」モンタージュ

```
A cinematic montage of micro-moments showing a Japanese woman in
her late 20s over time. Smooth crossfade between four scenes,
each 2 seconds: 1) opening a laptop at home at night with focused
expression, 2) handwriting notes at a cafe in daylight, 3) on a
video call smiling, 4) closing the laptop with a soft satisfied
breath. Consistent warm beige palette, natural window light
throughout. Documentary handheld feel, slight motion. Loops
seamlessly back to scene 1.

Audio: gentle piano-led ambient music, soft, no vocals.

Duration: 8 seconds. Aspect: 16:9.
```

## V-03 「コーチング 1on1」

```
Over-the-shoulder cinematic shot. A Japanese woman in her late
20s on a video call with her career coach (other person visible
on the laptop screen, also a Japanese woman in early 30s). Both
smile and engage in conversation. The student takes a small note,
nods. Camera static, slight shallow focus on the laptop. Background
is a warm-lit Tokyo home with a plant and beige decor. Window
light. Smooth seamless loop.

Audio: faint laptop fan, soft muffled voices (no clear words),
gentle paper rustle.

Duration: 8 seconds. Aspect: 16:9.
```

## V-04 「画面の中で完成していくデザイン」

```
A screen-recording-style cinematic shot of a clean simple
Figma-like canvas (no real brand UI). Shapes, type, and images
appear one by one to compose a small banner design for a fictional
neighborhood cafe. Smooth ease-in animation for each element.
Cream/beige/terracotta color palette. The camera (the screen) is
static. Loops back to empty canvas seamlessly.

Audio: subtle soft UI clicks, gentle keyboard taps, ambient room
tone.

Duration: 8 seconds. Aspect: 16:9.
```

---

# 制作プラン（推奨フロー）

## Phase 1: FVのみ先行制作（半日〜1日）

1. ImageFX で **A-01 / A-02 / A-03** を生成（各3〜5バリエーション、計9〜15枚）
2. 一番反応が良さそうな1枚をベースに、A-01 主役モデルの「顔の特徴」をメモ
3. その世界観で広告クリエイティブを先にテスト（Meta / Instagram）

## Phase 2: ストーリー4カット（1日）

1. C-01〜C-04 を **A-01 と同じ「中村早紀像」モデル**で生成
2. ImageFX の場合は同じシード（または "the same Japanese woman from previous image"）を活用
3. Phase 1で決めた配色・光・服装の方向性を全カットで統一

## Phase 3: 残りの素材（1〜2日）

1. F-01〜F-04（顔写真4名）→ F-01 は C-01〜04 と同人物
2. D-01〜D-03（ベネフィット帯）
3. E-01〜E-08（スキル静物）
4. B-01 / B-02 / G-01

## Phase 4: 動画4本（1日）

1. **V-01（FV直下）を必ず先に作る** — これがあるとFVの滞在時間が伸びる
2. 残り3本（V-02 / V-03 / V-04）は LP 中盤・終盤で使う
3. FLOW で各 8 秒×3-5パターン生成 → 一番自然なものを採用

---

# モデル一貫性のコツ（ImageFX編）

ImageFX は seed 固定がUIにないため、人物一貫性の維持にコツが必要：

1. **ベース画像を1枚決める**（A-01）
2. プロンプトに **「the same Japanese woman in her late 20s with [特徴]」** を含める
3. 特徴を箇条書きで毎回入れる：
   - 髪型 (low ponytail / messy bun / loose layers)
   - 顔の輪郭 (oval face with soft jawline)
   - 目元 (gentle almond-shaped eyes)
   - 体型 (slim build, average height)
   - スタイル (minimalist beige and cream wardrobe)
4. Style Modifiersは毎回統一：`35mm documentary, warm desaturated, beige palette, soft window light`

それでも完全一致しない場合は：
- **Nano Banana** でベース画像を入力にして「same person, different pose」生成
- **Runway** の Reference 機能
- 撮影で揃える（最終手段）

---

# FLOW（Veo 3）の特徴・コツ

- **音声生成も含む** ので、Audioを書かないと無音、書くと環境音生成
- **Camera movement** を明示すると効く: "static camera", "slow dolly in", "handheld slight shake"
- **Lighting** を必ず: "warm window light", "golden hour", "single lamp light"
- **8秒以上** は分割生成 → 編集ツールで繋ぐ（FLOWは1カット8秒上限）
- ループ用には文末に **"loops seamlessly back to start position"** と書く
- **音楽は著作権リスク** があるため、"ambient", "no music", "subtle piano-led ambient" 程度に留める

---

# まとめ：あなたが今すぐやること

| やること | 工数 | 成果物 |
|---|---|---|
| 1. ImageFX で A-01 を 5パターン生成 | 30分 | FV候補画像 |
| 2. 一番刺さるトーンを決める | 15分 | スタイル基準 |
| 3. C-01 を同じモデルで生成 | 30分 | ストーリー1カット目（連続性検証） |
| 4. 連続性が出てたら全素材生成へ進む | 2-3日 | 17画像+4動画 |

**最初に作るべき1枚は A-01 です**。これが世界観のすべてを決めます。
