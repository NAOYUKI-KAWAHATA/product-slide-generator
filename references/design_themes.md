# デザインテーマ一覧 v1

> LP画像から抽出した8つのデザインテーマ。
> **レイアウト**は常に `canva_reference/` のCanvaテンプレートを参照する（固定）。
> **世界観（色・装飾・雰囲気）**のみ、このファイルのテーマプロンプトで上書きする。
>
> 使い方: `design_system.md` の `COLOR PALETTE` と `DECORATIVE ELEMENTS` のセクションを、
> 選択されたテーマの `=== THEME OVERRIDE ===` ブロックで置き換える。

---

## テーマ一覧

| # | テーマID | テーマ名 | 雰囲気 | 向いているジャンル |
|---|---|---|---|---|
| 1 | `gemini_gradient` | Gemini グラデーション | 白ベース＋青紫グラデーション＋ガラスモーフィズム | AI・テック・ビジネス |
| 2 | `beige_brown` | ベージュブラウン | 暖かみのあるブラウン＋ゴールド光線 | ビジネス・マーケティング・男性向け |
| 3 | `cosmic_navy` | コスミックネイビー | 深いネイビー＋ゴールド＋スポットライト | 高級感・権威・男性向け |
| 4 | `forest_green` | フォレストグリーン | ベージュ＋深緑＋植物装飾 | 子育て・教育・ナチュラル |
| 5 | `luxury_gold` | ラグジュアリーゴールド | 白＋シャンパンゴールド＋水滴装飾 | 美容・ライフスタイル・女性向け |
| 6 | `rose_red` | ローズレッド | 深紅＋薔薇の花装飾＋ローズゴールド | スピリチュアル・恋愛・女性向け |
| 7 | `light_pastel` | ライトパステル | 白＋水色＋ピンク＋ダイヤモンド装飾 | 美容・ファッション・爽やか |
| 8 | `aqua_blue` | アクアブルー | ティール＋水色＋水紋装飾 | 健康・美容・ヨガ・ピラティス |

**LP参照画像パス**: `/home/ubuntu/skills/product-slide-generator/templates/themes/`

---

## テーマ1: Gemini グラデーション（既存・デフォルト）

**テーマID**: `gemini_gradient`
**LP参照画像**: なし（既存のdesign_system.mdがそのまま適用される）

```
=== THEME OVERRIDE: GEMINI GRADIENT ===

BACKGROUND:
- Base: pure white (#FFFFFF) to very light warm gray (#F8F7F5)
- Subtle white marble texture in background
- Corner decorations: thin blue-purple gradient geometric lines
- Overall: bright, airy, premium tech aesthetic

COLOR PALETTE:
- Background: white (#FFFFFF) to light gray (#F8F7F5)
- Primary text: dark charcoal (#333333)
- Title accent: blue-purple gradient (#6B8DD6 to #8E6BC6)
- Accent lines: blue-purple (#7B7FC4)
- Glassmorphism panels: rgba(255,255,255,0.6) with blur effect
- Header banner: dark charcoal (#333333) with white text

DECORATIVE ELEMENTS:
- Glassmorphism center panel with frosted glass effect
- Thin blue-purple gradient border lines at corners
- Subtle geometric grid pattern in background
- Clean, tech-forward aesthetic

MOOD: Sophisticated AI/tech premium — like a high-end software product launch
```

---

## テーマ2: ベージュブラウン

**テーマID**: `beige_brown`
**LP参照画像**: `theme_02_beige_brown.jpg`

```
=== THEME OVERRIDE: BEIGE BROWN ===

BACKGROUND:
- Base: warm beige (#F5EDD8) to light cream (#FAF3E0)
- Subtle warm texture, like aged parchment
- Corner decorations: golden light ray streaks emanating from top-right
- Overall: warm, confident, masculine authority

COLOR PALETTE:
- Background: warm beige (#F5EDD8) to cream (#FAF3E0)
- Primary text: dark brown (#3D2B1F)
- Title text: warm white (#FFFFFF) with dark brown background band
- Accent: warm gold (#C8A96E)
- Highlight bands: dark chocolate brown (#4A2E1A) horizontal stripes behind titles
- Header banner: dark chocolate brown (#4A2E1A) with white text

DECORATIVE ELEMENTS:
- Golden light rays / sunburst effect from upper-right corner
- Dark brown horizontal band behind main title text (full width)
- Warm gold circular badge element in lower-right
- Subtle warm bokeh light effects in background
- Rounded rectangle info box in warm gold at bottom

MOOD: Warm authority and confidence — like a premium business seminar for driven professionals
```

---

## テーマ3: コスミックネイビー

**テーマID**: `cosmic_navy`
**LP参照画像**: `theme_03_cosmic_navy.jpg`

```
=== THEME OVERRIDE: COSMIC NAVY ===

BACKGROUND:
- Base: deep navy blue (#0D1B3E) to dark midnight blue (#0A1628)
- Subtle star/cosmos texture in background
- Spotlight effect from upper-right: warm golden light beam
- Overall: powerful, authoritative, premium night-sky aesthetic

COLOR PALETTE:
- Background: deep navy (#0D1B3E) to midnight blue (#0A1628)
- Primary text: white (#FFFFFF)
- Title text: white (#FFFFFF) with champagne gold (#C8A96E) accent
- Accent: champagne gold (#C8A96E) and bright gold (#FFD700)
- Divider lines: champagne gold (#C8A96E)
- Header banner: dark navy (#0A1628) with gold border and white text

DECORATIVE ELEMENTS:
- Warm golden spotlight beam from upper-right corner
- Champagne gold thin border frame around entire slide
- Gold circular badge/seal element in lower-right corner
- Subtle star/particle effects in dark background
- Rounded rectangle info box: dark navy with gold border

MOOD: Cosmic authority and premium exclusivity — like a VIP invitation to an elite event
```

---

## テーマ4: フォレストグリーン

**テーマID**: `forest_green`
**LP参照画像**: `theme_04_forest_green.jpg`

```
=== THEME OVERRIDE: FOREST GREEN ===

BACKGROUND:
- Base: warm cream (#F5F0E8) to soft beige (#EDE8DC)
- Watercolor wash effect in corners: soft sage green (#C8D5B9)
- Botanical decorations: hand-drawn style leaves, small flowers, branches
- Overall: natural, warm, nurturing, organic aesthetic

COLOR PALETTE:
- Background: warm cream (#F5F0E8) to soft beige (#EDE8DC)
- Primary text: deep forest green (#1A4A2E)
- Title text: deep forest green (#1A4A2E), bold
- Accent: sage green (#6B9E78) and forest green (#2D6A4F)
- Divider lines: sage green (#6B9E78), hand-drawn style
- Header banner: forest green (#2D6A4F) with white text

DECORATIVE ELEMENTS:
- Hand-drawn botanical illustrations: leaves, small wildflowers, thin branches
- Watercolor green wash in corners and edges
- Rounded rectangle info box: cream with forest green border
- Circular badge: forest green with laurel wreath decoration
- Organic, imperfect lines — NOT geometric or corporate

MOOD: Warm, nurturing, natural growth — like a caring educator in a sunlit garden
```

---

## テーマ5: ラグジュアリーゴールド

**テーマID**: `luxury_gold`
**LP参照画像**: `theme_05_luxury_gold.jpg`

```
=== THEME OVERRIDE: LUXURY GOLD ===

BACKGROUND:
- Base: pure white (#FFFFFF) to very light warm cream (#FDF9F0)
- Soft bokeh light effects: warm golden circles, subtle and dreamy
- Right side: flowing champagne gold ribbon/stream decoration
- Water droplet accents: small golden drops scattered elegantly
- Overall: feminine luxury, spa-like, premium beauty aesthetic

COLOR PALETTE:
- Background: white (#FFFFFF) to light cream (#FDF9F0)
- Primary text: dark warm brown (#3D2B1F)
- Title text: champagne gold (#C8A96E) with subtle shimmer
- Accent: champagne gold (#C8A96E) and warm gold (#D4AF6A)
- Divider lines: champagne gold (#C8A96E), thin and delicate
- Header banner: champagne gold (#C8A96E) with dark brown text

DECORATIVE ELEMENTS:
- Flowing champagne gold ribbon/stream on right side of slide
- Small golden water droplets scattered in background
- Soft warm bokeh circles in background
- Diamond/rhombus shaped badge in upper-right: gold outline with text inside
- Circular clock/date badge: gold ring with white interior
- Thin gold horizontal band at bottom for info

MOOD: Feminine luxury and elegance — like a premium spa or high-end beauty brand
```

---

## テーマ6: ローズレッド

**テーマID**: `rose_red`
**LP参照画像**: `theme_06_rose_red.jpg`

```
=== THEME OVERRIDE: ROSE RED ===

BACKGROUND:
- Base: deep crimson red (#8B1A2F) to dark burgundy (#6B0F1F)
- Large rose flower illustrations: semi-transparent, overlapping in corners
- Subtle golden star/sparkle particles scattered throughout
- Overall: passionate, mystical, romantic, spiritual aesthetic

COLOR PALETTE:
- Background: deep crimson (#8B1A2F) to dark burgundy (#6B0F1F)
- Primary text: white (#FFFFFF)
- Title text: white (#FFFFFF) with warm glow
- Accent: rose gold (#C9956C) and warm gold (#D4AF6A)
- Divider lines: rose gold (#C9956C)
- Header banner: dark burgundy (#6B0F1F) with rose gold border and white text

DECORATIVE ELEMENTS:
- Large semi-transparent rose flower illustrations in corners (top-right, bottom-left)
- Golden sparkle/star particles scattered throughout background
- Circular badge: rose gold ring with laurel wreath, white text inside
- Rounded rectangle info box: dark burgundy with rose gold border
- Circular rose icon/emblem in upper-left area

MOOD: Passionate mystique and feminine power — like a high-end spiritual or romance coaching brand
```

---

## テーマ7: ライトパステル

**テーマID**: `light_pastel`
**LP参照画像**: `theme_07_light_pastel.jpg`

```
=== THEME OVERRIDE: LIGHT PASTEL ===

BACKGROUND:
- Base: very light lavender (#F0EEFF) to soft sky blue (#E8F4FF) gradient
- Floating geometric shapes: translucent diamond/crystal shapes in pastel blue and pink
- Dot matrix pattern in upper-right corner: subtle gray dots
- Overall: fresh, youthful, digital-native, clean aesthetic

COLOR PALETTE:
- Background: light lavender (#F0EEFF) to sky blue (#E8F4FF)
- Primary text: dark navy (#1A2A4A)
- Title text: gradient from sky blue (#5BB8F5) to soft pink (#F5A0C0)
- Accent: sky blue (#5BB8F5) and soft pink (#F5A0C0)
- Divider lines: light blue (#A0D4F5), thin
- Header banner: light blue (#5BB8F5) with white text, rounded corners

DECORATIVE ELEMENTS:
- Floating translucent diamond/crystal shapes in pastel blue and pink
- Subtle dot matrix grid in upper-right corner
- Rounded rectangle info box: white with light blue border
- Circular badge: light blue-pink gradient with white text
- Sparkle star accents near header text
- Clean, airy geometric decorations

MOOD: Fresh digital confidence — like a modern beauty tech or lifestyle app brand
```

---

## テーマ8: アクアブルー

**テーマID**: `aqua_blue`
**LP参照画像**: `theme_08_aqua_blue.jpg`

```
=== THEME OVERRIDE: AQUA BLUE ===

BACKGROUND:
- Base: soft aqua (#C8EEF0) to light teal (#B0E8EC) gradient
- Water ripple/ring patterns: concentric circles in slightly darker teal
- Water droplet accents: transparent drops scattered elegantly
- Bubble elements: small transparent circles floating
- Overall: refreshing, clean, health-focused, wellness aesthetic

COLOR PALETTE:
- Background: soft aqua (#C8EEF0) to light teal (#B0E8EC)
- Primary text: dark teal (#1A5F6A)
- Title text: deep teal (#1A5F6A), bold
- Accent: medium teal (#2E9DAA) and silver (#B0C4C8)
- Divider lines: medium teal (#2E9DAA)
- Header banner: medium teal (#2E9DAA) with white text, pill/rounded shape

DECORATIVE ELEMENTS:
- Concentric water ripple rings in background (subtle, darker teal)
- Small transparent water droplets and bubbles scattered throughout
- Rounded rectangle info box: light teal with medium teal border, rounded corners
- Circular badge: silver/chrome ring with white interior and teal text
- Water drop icon accent near header elements
- Pill-shaped tag/label for header text (rounded ends)

MOOD: Refreshing wellness and clarity — like a premium spa, yoga studio, or health brand
```

---

## 全テーマ共通: テキスト色ルール（必ず遵守）

> **このルールは全テーマに適用される。テーマの `=== THEME OVERRIDE ===` より優先する。**

```
=== UNIVERSAL TEXT COLOR RULES (OVERRIDES ALL THEMES) ===

TEXT COLOR BY PAGE TYPE:
- Cover page (cover): main title → gold or theme accent color OK
- Section divider (section-title): section title → gold or theme accent color OK
- ALL OTHER PAGES: body text, bullet points, descriptions → MUST be charcoal gray (#333333) or white (#FFFFFF) only

GRADIENT TEXT RESTRICTION:
- Gradient text is ONLY allowed on: cover page title, section divider title
- NEVER use gradient text on: bullet points, descriptions, sub-headings, captions, any body copy
- Reason: gradient body text looks AI-generated and cheap

DECORATIVE ELEMENTS vs TEXT:
- Banners, borders, divider lines, background elements: theme colors and gradients are OK
- Text content: charcoal (#333333) or white (#FFFFFF) ONLY (except cover/section titles)

ANTI-GLITTER MANDATE:
- The overall impression must be: "This looks expensive and professionally designed"
- NOT: "This looks like an AI made it with too many effects"
- Maximum ONE decorative technique per slide
- All effects must be subtle enough to be barely noticeable at first glance
```

---

## 使用方法（Manusへの指示）

スライド生成時、ユーザーが選択したテーマに応じて以下の手順でプロンプトを構成する。

**Step 1**: 選択テーマの `=== THEME OVERRIDE ===` ブロックを取得する。

**Step 2**: `design_system.md` の共通プロンプトの `COLOR PALETTE` と `DECORATIVE ELEMENTS` セクションをテーマのものに置き換える。

**Step 3**: 各ページのプロンプトに以下の順で `references` を指定する：
1. 対応するCanvaレイアウト参照画像（`canva_reference/` フォルダ）— レイアウト構造の参照
2. 選択テーマのLP参照画像（`themes/` フォルダ）— 色・雰囲気の参照
3. 直前ページの生成画像（2ページ目以降）— デザイン継続性の参照

**Step 4**: プロンプト内に明示する：
```
IMPORTANT: Follow the LAYOUT from the Canva reference image.
Follow the COLOR and ATMOSPHERE from the theme reference image.
Do NOT copy the text content from either reference image.
```
