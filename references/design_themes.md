# デザインテーマ一覧 v2

> **重要**: このファイルは各テーマの「世界観」を定義する。
> **レイアウト（構造）**は全テーマ共通で `canva_reference/` の画像に従う（固定）。
> **世界観（色・装飾・雰囲気）**のみ、このファイルのテーマプロンプトで上書きする。
>
> 使い方: `design_system.md` の `COLOR PALETTE` と `DECORATIVE ELEMENTS` のセクションを、
> 選択されたテーマの `=== THEME OVERRIDE ===` ブロックで置き換える。

---

## テーマ一覧

| # | テーマID | テーマ名 | 背景 | タイトル文字 | 向いているジャンル |
|---|---|---|---|---|---|
| 1 | `light_pastel` | ライトパステル | 白〜淡いピンク〜ラベンダー | ブルー→パープル→ピンクのグラデーション | 美容・ファッション・女性向け |
| 2 | `aqua_blue` | アクアブルー | ホワイトベース | ブルーグラデーション | 健康・美容・ヨガ・コンサル |
| 3 | `forest_green` | フォレストグリーン | 淡いグリーングラデーション | 深緑アクセント | 子育て・教育・ナチュラル |
| 4 | `geometric` | ジオメトリック | ホワイトグレー＋幾何学線 | ブルー→パープル→ピンクのグラデーション | AI・テック・ビジネス |
| 5 | `soft_beige` | ソフトベージュ | 薄いホワイトベージュ | ベージュグラデーション | ライフスタイル・コーチング・女性向け |

**テーマ参照画像パス**: `templates/themes/theme_XX_<name>/`
各テーマフォルダに `cover.png`, `content.png`, `bullet_list.png`, `pricing.png` を格納。

---

## 共通ルール（全テーマ必須・テーマ指定より優先）

### テキスト色ルール
- **本文・箇条書き・説明文**: チャコールグレー（#333333〜#4A4A4A）または白（暗い背景の場合）
- **扉タイトル・大見出しのみ**: テーマ指定のグラデーション文字OK
- **それ以外のページのタイトル**: チャコールグレーまたは白。グラデーション文字禁止
- **見出しバナー・装飾**: テーマカラーのグラデーションOK

### ギラギラ禁止ルール（ANTI-GLITTER MANDATE）
- 1スライドに使う装飾技法は最大1種類
- 全ての装飾は「一見気づかないくらい控えめ」に
- 判定基準：「洗練された高級感がある」→ OK / 「AIっぽい・ギラギラ」→ NG
- 光沢・グロー・レンズフレアは最小限に抑える
- 背景のグラデーションは柔らかく自然な遷移にする

### 見出しバナー統一ルール
- 見出しが必要なページ → 同一デザインのバナー＋白文字を必ず使う
- 扉・表紙・インパクト文ページ → 見出しバナーなし
- **異なるデザインの見出しが複数出てくることは絶対NG**

---

## テーマ1: ライトパステル（Light Pastel）

**テーマID**: `light_pastel`
**リファレンス画像**: `templates/themes/theme_01_light_pastel/`

```
=== THEME OVERRIDE: LIGHT PASTEL ===

BACKGROUND:
- Base: white (#FFFFFF) with very subtle gradient to pale pink (#FFF0F5) and pale lavender (#F0E6FF)
- Soft, diffused light glow in bottom-right corner
- Overall: ethereal, soft, premium feminine aesthetic

COLOR PALETTE:
- Background: white → pale pink (#FFF0F5) → pale lavender (#F0E6FF)
- Primary text: charcoal gray (#4A4A4A)
- Title text (cover/section ONLY): blue-to-purple-to-pink gradient (#4A90D9 → #8B5CF6 → #EC4899). Serif typeface.
- Accent: subtle gold (#C5A55A) for price highlights only
- Heading banner: soft pink-to-lavender gradient (#F0A0C0 → #C0A0E0) with white text
- Bullet icons: diamond (◆) shape in gradient pink-purple

DECORATIVE ELEMENTS:
- Thin diamond-shaped geometric lines, very subtle
- Controlled light particles — barely visible, like dust in sunlight
- NO heavy glow, NO lens flare, NO sparkle clusters
- Clean and delicate — like fine jewelry packaging

MOOD: Like a luxury jewelry brand lookbook — delicate, precious, aspirational
```

---

## テーマ2: アクアブルー（Aqua Blue）

**テーマID**: `aqua_blue`
**リファレンス画像**: `templates/themes/theme_02_aqua_blue/`

```
=== THEME OVERRIDE: AQUA BLUE ===

BACKGROUND:
- Base: clean white (#FFFFFF to #F8FBFF)
- Very subtle blue tint at edges or corners
- Overall: clean, professional, trustworthy

COLOR PALETTE:
- Background: white (#FFFFFF) to very light blue (#F8FBFF)
- Primary text: charcoal gray (#333333)
- Title text (cover/section ONLY): blue gradient (#1E90FF → #0066CC → #003D7A). Sans-serif typeface.
- Accent: deep navy (#0D47A1) for emphasis, light blue (#E3F2FD) for background highlights
- Heading banner: blue gradient (#2196F3 → #0D47A1) with white text
- Bullet icons: circle or square in solid blue (#2196F3)

DECORATIVE ELEMENTS:
- Subtle water ripple or wave patterns — very faint, background only
- Clean geometric lines if any — thin and precise
- NO heavy water effects, NO bubble clusters
- Minimal and professional

MOOD: Like a premium consulting firm presentation — authoritative, clean, trustworthy
```

---

## テーマ3: フォレストグリーン（Forest Green）

**テーマID**: `forest_green`
**リファレンス画像**: `templates/themes/theme_03_forest_green/`

```
=== THEME OVERRIDE: FOREST GREEN ===

BACKGROUND:
- Base: soft green gradient (#F0F7F0 → #E8F5E8 → #D4EDDA)
- Very gentle, like morning light through leaves
- Subtle botanical silhouettes at edges — faint and understated
- Overall: natural, warm, nurturing, organic luxury

COLOR PALETTE:
- Background: soft green gradient (#F0F7F0 → #E8F5E8 → #D4EDDA)
- Primary text: dark charcoal (#333333)
- Title text (cover/section ONLY): deep forest green gradient (#2D5016 → #1B5E20 → #388E3C). Elegant serif or sans-serif.
- Accent: warm gold (#B8860B) for price highlights. Soft cream (#FFF8E1) for card backgrounds
- Heading banner: deep green gradient (#2E7D32 → #1B5E20) with white text
- Bullet icons: leaf (🍃) or circle in forest green (#2E7D32)

DECORATIVE ELEMENTS:
- Subtle botanical elements — faint leaf silhouettes, gentle vine patterns at edges
- Watercolor-like green wash in corners — very understated
- NO heavy floral illustrations, NO cartoon plants
- Organic and imperfect — hand-drawn feel, not corporate geometric

MOOD: Like a premium organic spa brochure — calming, trustworthy, grounded in nature
```

---

## テーマ4: ジオメトリック（Geometric）

**テーマID**: `geometric`
**リファレンス画像**: `templates/themes/theme_04_geometric/`

```
=== THEME OVERRIDE: GEOMETRIC ===

BACKGROUND:
- Base: white to light gray (#FFFFFF → #F5F5F7)
- Subtle geometric line patterns: thin intersecting lines, hexagons, or angular shapes in very light gray (#E0E0E0)
- Lines are outlines only — NO fills, NO solid shapes
- Overall: modern, intellectual, structured, tech-meets-art

COLOR PALETTE:
- Background: white (#FFFFFF) to light gray (#F5F5F7)
- Primary text: charcoal gray (#333333)
- Title text (cover/section ONLY): blue-to-purple-to-pink gradient (#4A90D9 → #7C3AED → #EC4899). Modern sans-serif.
- Accent: purple (#7C3AED) for emphasis. Light lavender (#F3E8FF) for background highlights
- Heading banner: blue-to-purple gradient (#4A90D9 → #7C3AED) with white text
- Bullet icons: geometric shapes — hexagon or triangle in gradient blue-purple

DECORATIVE ELEMENTS:
- Thin geometric wireframe lines — angular, precise, architectural
- Outlines only — NO filled shapes, NO heavy patterns
- Very subtle — like a faint blueprint in the background
- NO neon glow, NO 3D effects

MOOD: Like a cutting-edge tech company keynote — structured, forward-thinking, intellectual
```

---

## テーマ5: ソフトベージュ（Soft Beige）

**テーマID**: `soft_beige`
**リファレンス画像**: `templates/themes/theme_05_soft_beige/`

```
=== THEME OVERRIDE: SOFT BEIGE ===

BACKGROUND:
- Base: pale white-beige (#FFFBF5 → #FFF5E6)
- Organic, irregular-shaped frames in very pale yellow (#FFF9C4) and soft orange (#FFE0B2)
- Shapes are like watercolor blobs — soft, flowing, NOT geometric
- Overall: warm, approachable, soft luxury

COLOR PALETTE:
- Background: pale white-beige (#FFFBF5 → #FFF5E6)
- Primary text: warm charcoal (#4A4040)
- Title text (cover/section ONLY): warm beige-to-gold gradient (#C4A265 → #8B7355 → #A0845C). Elegant serif.
- Accent: muted orange (#E8A87C) for highlights. Cream (#FFF8E1) for card backgrounds
- Heading banner: warm beige-gold gradient (#C4A265 → #8B7355) with white text
- Bullet icons: soft circle or dot in warm gold (#C4A265)

DECORATIVE ELEMENTS:
- Organic, irregular blob shapes in very pale yellow and soft peach as background frames
- Watercolor-like soft edges — flowing, imperfect, natural
- NO sharp geometric lines, NO angular patterns
- Warm and inviting — like a hand-painted watercolor border

MOOD: Like a premium lifestyle magazine spread — warm, inviting, effortlessly stylish
```

---

## テーマ選択時の運用ルール

1. ユーザーにテーマ一覧を提示し、番号で選択してもらう
2. 選択されたテーマの「世界観プロンプト」を全スライド生成に適用する
3. 各スライド生成時、テーマフォルダ内の最も近いリファレンス画像を必ず添付する
   - 表紙 → `cover.png`
   - 箇条書き・リスト系 → `bullet_list.png`（ない場合は `content.png`）
   - コンテンツ説明系 → `content.png`
   - 価格・比較系 → `pricing.png`
4. レイアウト構造は `canva_reference/` の画像に従う（テーマに関係なく共通）
5. テーマ画像はあくまで「色・装飾・雰囲気」の参考。レイアウトはCanvaテンプレートが優先

### リファレンス画像の指定順序（references配列）
1. 対応するCanvaレイアウト参照画像（`canva_reference/` フォルダ）— レイアウト構造の参照
2. 選択テーマのリファレンス画像（`themes/theme_XX/` フォルダ）— 色・雰囲気の参照
3. 直前ページの生成画像（2ページ目以降）— デザイン継続性の参照

### プロンプト内に明示する文言
```
IMPORTANT: Follow the LAYOUT from the Canva reference image.
Follow the COLOR and ATMOSPHERE from the theme reference image.
Do NOT copy the text content from either reference image.
```
