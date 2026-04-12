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
| 6 | `natural_pink` | ナチュラルピンク | 白ベース＋水彩ピンク | ローズピンクグラデーション | 女性向けサロン・恋愛・婚活 |
| 7 | `navy_gold` | ネイビーゴールド | ネイビーブルーグラデーション | 白文字 | 男性向け・ビジネス系 |
| 8 | `gray_gold` | グレーゴールド | グレーグラデーション | ゴールド（メタリック） | 男性向け・ビジネス・コンサル |

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

TYPOGRAPHY (CRITICAL — OVERRIDES DEFAULT):
- ALL text on ALL pages MUST use a feminine Japanese serif (Mincho) typeface — elegant, thin strokes
- NEVER use Gothic (sans-serif) typeface anywhere — not for titles, not for body, not for banners
- Heading banner text: white Mincho serif
- Body text: charcoal gray Mincho serif
- Title text: dusty gradient Mincho serif

BACKGROUND:
- Cover page: soft pink to near-white to lavender gradient (#F5E3F3 → #FFFCFE → #EBEAF8)
- Content pages: same gradient, slightly lighter — barely perceptible, the page should read as "white with a whisper of color"
- Overall: delicate, feminine, refined elegance

COLOR PALETTE:
- Background: #F5E3F3 → #FFFCFE → #EBEAF8 (pink → near-white → lavender)
- Primary text: charcoal gray (#4A4A4A)
- Title text (cover/section ONLY): blue-to-purple-to-pink gradient (#6F9DC2 → #9F82C8 → #D68EC6). Muted, sophisticated.
- Accent: subtle gold (#C5A55A) for price highlights only
- Heading banner: soft dusty pink-to-lavender gradient (#D4A0B0 → #B0A0C8) with white text
- Bullet icons: diamond (◆) shape in dusty pink-purple

DECORATIVE ELEMENTS:
- DIAGONAL LINES in top-left and bottom-right corners — hair-thin strokes, barely visible
- Line color: 5-color grey gradient (#6E6969 → #FFFFFF → #818181 → #F5F5F5 → #797878)
- 2 lines per corner (one slightly thicker at 2px, one at 1px with 0.7 opacity)
- Lines are rotated at -45 degrees, extending beyond the corner edge
- NO sparkle, NO glow, NO light particles — completely removed
- NO diamond shapes — diagonal lines only
- Keep the center clean and open
- Delicate and feminine — like fine lace or silk texture

TEXT SPACING (CRITICAL FOR CONTENT PAGES):
- Generous line spacing between bullet points — each line should breathe with ample whitespace above and below
- 3-line bullet lists should be evenly distributed across the vertical center of the slide with wide gaps between lines
- Text should feel spacious and airy, never cramped or dense
- Minimum 60px visual gap between each bullet line

MOOD: Delicate feminine elegance — like a luxury bridal magazine. Refined, soft, never loud. Every element whispers rather than shouts.
```

### テーマ1 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSで実装する。

```
BG_COLOR: #FFFCFE
BG_GRADIENT: linear-gradient(135deg, #F5E3F3 0%, #FFFCFE 50%, #EBEAF8 100%)
BG_GRADIENT_DARK: linear-gradient(135deg, #F5E3F3 0%, #FFFCFE 50%, #EBEAF8 100%)
TITLE_GRADIENT_CSS: background: linear-gradient(90deg, #6F9DC2, #9F82C8, #D68EC6); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
TITLE_COLOR: #9F82C8
SUBTITLE_COLOR: #9F82C8
TEXT_COLOR: #4A4A4A
BULLET_COLOR: #D68EC6
BULLET_CHAR: ◆
BANNER_BG: linear-gradient(90deg, #6F9DC2, #9F82C8, #D68EC6)
BANNER_BG_WIDE: linear-gradient(90deg, #6F9DC2, #9F82C8, #D68EC6)
RULE_COLOR: rgba(159, 130, 200, 0.4)
LINE_COLOR: linear-gradient(90deg, #6F9DC2, #9F82C8, #D68EC6)
DECO_LINE_GRADIENT: linear-gradient(90deg, #6E6969, #FFFFFF, #818181, #F5F5F5, #797878)
PRICE_COLOR: #C5A55A
```

---
【装飾 — 全ページ共通（表紙・コンテンツ）用】
左上・右下に5色グレーグラデーションの斜め線（CSS で実装）。キラキラ・光の粒は使用禁止。

```html
<!-- 左上の斜め線装飾 -->
<div style="position:absolute;top:-50px;left:-50px;width:300px;height:300px;z-index:0;pointer-events:none;">
  <div style="position:absolute;top:150px;left:-100px;width:400px;height:2px;background:linear-gradient(90deg, #6E6969, #FFFFFF, #818181, #F5F5F5, #797878);transform:rotate(-45deg);"></div>
  <div style="position:absolute;top:200px;left:-50px;width:400px;height:1px;background:linear-gradient(90deg, #6E6969, #FFFFFF, #818181, #F5F5F5, #797878);transform:rotate(-45deg);opacity:0.7;"></div>
</div>

<!-- 右下の斜め線装飾 -->
<div style="position:absolute;bottom:-50px;right:-50px;width:300px;height:300px;z-index:0;pointer-events:none;">
  <div style="position:absolute;bottom:150px;right:-100px;width:400px;height:2px;background:linear-gradient(90deg, #6E6969, #FFFFFF, #818181, #F5F5F5, #797878);transform:rotate(-45deg);"></div>
  <div style="position:absolute;bottom:200px;right:-50px;width:400px;height:1px;background:linear-gradient(90deg, #6E6969, #FFFFFF, #818181, #F5F5F5, #797878);transform:rotate(-45deg);opacity:0.7;"></div>
</div>
```

---

## テーマ2: アクアブルー（Aqua Blue）

**テーマID**: `aqua_blue`
**リファレンス画像**: `templates/themes/theme_02_aqua_blue/`

```
=== THEME OVERRIDE: AQUA BLUE ===

TYPOGRAPHY (CRITICAL — OVERRIDES DEFAULT):
- ALL text on ALL pages MUST use a Japanese serif (Mincho) typeface — elegant, refined
- NEVER use Gothic (sans-serif) typeface anywhere
- Heading banner text: white Mincho serif
- Body text: charcoal gray (#4A4A4A) Mincho serif
- Title text: teal-to-navy gradient Mincho serif

BACKGROUND:
- Cover page ONLY: PURE WHITE (#FFFFFF) — completely clean, no tint at all
- Content pages: very pale mint-green to ice-blue tint (#F0F8F8 / #EFF8F8) — almost white but with a whisper of cool color
- Overall: clean, intellectual, trustworthy

COLOR PALETTE:
- Cover background: pure white (#FFFFFF)
- Content background: pale mint-ice (#F0F8F8)
- Primary text: charcoal gray (#4A4A4A)
- Title text (cover/section ONLY): teal (#2A8A8A) → navy (#1A3A5C) gradient. Mincho serif.
- Title underline: thin horizontal line in teal-to-navy gradient, placed directly below the title text
- Accent: teal (#2A8A8A) for emphasis labels like "提供内容", warm gold (#B8A060) for price highlight bands
- Heading banner (small, コンセプト style): teal → lavender gradient (#5AACAC → #8A8ABF) with white text, compact rectangle at top-left
- Heading banner (large, この講座から得られる未来 style): wider teal → lavender gradient band across upper area, centered white text
- Bullet icons: none (text only, or subtle dash)

DECORATIVE ELEMENTS:
- LEFT EDGE: thin vertical gradient stripe running along the left border — teal (#5AACAC) at top fading to lavender (#9A8ABF) at bottom. Subtle, like a page edge accent.
- RIGHT-BOTTOM CORNER: only 2-3 delicate straight lines using the SAME teal-to-navy gradient as the title text (#2A8A8A → #1A3A5C). Hair-thin strokes, elegant and minimal. Lines should cross at gentle angles — NOT a busy cluster, but a refined accent like a calligraphy stroke.
- LESS IS MORE — do NOT add many lines. 2-3 lines maximum. The beauty is in the simplicity.
- These two decorative elements appear on EVERY page (cover and content) as consistent branding
- NO thick lines, NO bold strokes, NO busy patterns
- NO heavy effects, NO glow, NO sparkle
- Lines should feel like a refined signature — simple, elegant, sophisticated

TEXT SPACING (CRITICAL FOR CONTENT PAGES):
- Generous line spacing between bullet points — each line should breathe with ample whitespace
- 3-line lists should be evenly distributed across the vertical center with wide gaps
- Text should feel spacious and airy, never cramped

MOOD: Clean intellectual elegance — like a premium consulting firm or architectural studio. Sharp, precise, trustworthy. The intersecting lines give a sense of structure and sophistication.
```

### テーマ2 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSで実装する。

```
BG_COLOR: #F0F8F8
BG_GRADIENT: radial-gradient(ellipse at 50% 40%, #FFFFFF 0%, #F0F8F8 60%, #EAF4F4 100%)
BG_GRADIENT_DARK: linear-gradient(135deg, #2A8A8A 0%, #1A3A5C 100%)
TITLE_GRADIENT_CSS: background: linear-gradient(135deg, #2A8A8A, #1A3A5C); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
TITLE_COLOR: #2A8A8A
SUBTITLE_COLOR: #6A8A9A
TEXT_COLOR: #4A4A4A
BULLET_COLOR: #2A8A8A
BULLET_CHAR: —
BANNER_BG: linear-gradient(90deg, #5AACAC, #8A8ABF)
BANNER_BG_WIDE: linear-gradient(90deg, #5AACAC, #6A9ABF, #8A8ABF, #6A9ABF, #5AACAC)
RULE_COLOR: rgba(42, 138, 138, 0.3)
LINE_COLOR: linear-gradient(90deg, #2A8A8A, #1A3A5C)
PRICE_COLOR: #B8A060
```

---
【装飾 — 表紙（cover）用】
左端に縦のグラデーションストライプ、右下に2本の細い交差線。

```html
<!-- 左端縦グラデーションストライプ -->
<div style="position:absolute;top:0;left:0;width:6px;height:100%;background:linear-gradient(180deg,rgba(90,172,172,0.6) 0%,rgba(138,138,191,0.4) 100%);z-index:0;pointer-events:none;"></div>

<!-- 右下交差線 -->
<div style="position:absolute;bottom:60px;right:40px;width:160px;height:120px;z-index:0;pointer-events:none;">
  <div style="position:absolute;bottom:0;right:0;width:140px;height:2px;background:linear-gradient(90deg,rgba(42,138,138,0.5),rgba(26,58,92,0.5));transform:rotate(-30deg);transform-origin:right bottom;"></div>
  <div style="position:absolute;bottom:20px;right:0;width:120px;height:1px;background:linear-gradient(90deg,rgba(42,138,138,0.3),rgba(26,58,92,0.3));transform:rotate(-20deg);transform-origin:right bottom;"></div>
</div>
```

---
【装飾 — コンテンツページ用】
表紙と同じ左端ストライプ＋右下交差線（控えめ）。

```html
<!-- 左端縦グラデーションストライプ -->
<div style="position:absolute;top:0;left:0;width:5px;height:100%;background:linear-gradient(180deg,rgba(90,172,172,0.5) 0%,rgba(138,138,191,0.3) 100%);z-index:0;pointer-events:none;"></div>

<!-- 右下交差線（控えめ） -->
<div style="position:absolute;bottom:40px;right:30px;width:120px;height:90px;z-index:0;pointer-events:none;">
  <div style="position:absolute;bottom:0;right:0;width:100px;height:1px;background:linear-gradient(90deg,rgba(42,138,138,0.4),rgba(26,58,92,0.4));transform:rotate(-30deg);transform-origin:right bottom;"></div>
  <div style="position:absolute;bottom:15px;right:0;width:80px;height:1px;background:linear-gradient(90deg,rgba(42,138,138,0.25),rgba(26,58,92,0.25));transform:rotate(-20deg);transform-origin:right bottom;"></div>
</div>
```

---

## テーマ3: フォレストグリーン（Forest Green）

**テーマID**: `forest_green`
**リファレンス画像**: `templates/themes/theme_03_forest_green/`

```
=== THEME OVERRIDE: FOREST GREEN ===

TYPOGRAPHY (CRITICAL — OVERRIDES DEFAULT):
- ALL text on ALL pages MUST use a feminine Japanese serif (Mincho) typeface — elegant, thin strokes
- NEVER use Gothic (sans-serif) typeface anywhere — not for titles, not for body, not for banners
- Heading banner text: white Mincho serif
- Body text: dark charcoal-green (#3A4A3A) Mincho serif
- Title text: deep forest green GRADIENT (#2D5016 → #1B5E20 → #3A7A3A) Mincho serif

BACKGROUND:
- ALL PAGES (COVER AND CONTENT): ALMOST WHITE with a very subtle, fresh COOL mint-green tint (#EFF5F1 to #F5FAF7) — a clean, airy, COOL-toned sage-mint, like a gentle breeze through eucalyptus leaves.
- CRITICAL: ALL pages MUST use the SAME gradient background as the cover page. Content pages and pricing pages MUST NOT use a flat/solid color — they MUST have the same soft luminous gradient quality as the cover.
- CRITICAL COLOR RULE: The background MUST be primarily WHITE/VERY LIGHT. The green tint MUST have a BLUE/TEAL undertone. It should look like a mix of white and pale aqua/mint.
- ABSOLUTELY FORBIDDEN: yellow-green, olive-green, matcha, khaki, warm green, muddy green, army green, strong green, flat solid green. If the color looks like matcha powder, green tea, or is too saturated/dark, it is WRONG. A flat single-color background is also WRONG.
- Think: clean white space, cool eucalyptus breeze, sea foam, pale jade — NOT matcha, NOT olive, NOT moss, NOT heavy green.
- Slightly lighter in center (#FAFCFB), slightly deeper at edges (#EFF5F1) for subtle depth.
- Overall: clean, fresh, calming, airy, like a premium spa with lots of white space.
- APPROVED REFERENCE: The cover page generated image is the color standard. All subsequent pages MUST match that exact background tone.

COLOR PALETTE:
- Background: ALMOST WHITE with COOL mint-green tint (#EFF5F1 → #F5FAF7). Center lighter (#FAFCFB), edges deeper (#EFF5F1). MUST be very light and have blue/teal undertone — NEVER yellow-green, matcha, strong green, or flat solid color.
- Primary text: dark charcoal-green (#3A4A3A)
- Title text (cover/section ONLY): deep forest green GRADIENT (#2D5016 → #1B5E20 → #3A7A3A). Mincho serif. A rich green gradient that shifts from dark forest to slightly brighter green.
- Subtitle text: slightly lighter forest green (#4A6A3A)
- Accent: warm gold (#B8960B) for price highlights ONLY
- Heading banner (small, コンセプト style): muted olive-green to sage gradient (#8BA888 → #7A9A78) with white text, compact rectangle at top-left
- Heading banner (large, この講座から得られる未来 style): wider muted sage-green band, centered white text
- Bullet icons: none (text only, or subtle dash)

DECORATIVE ELEMENTS:
- COVER PAGE ONLY: watercolor-style botanical leaf silhouettes in EXTREMELY FAINT, cool gray-green (#B8C8C0 at ~15% opacity). Placed at TOP-LEFT corner (1-2 leaves cascading down) and BOTTOM-RIGHT corner (1-2 leaves). Leaves are soft, translucent, like pressed herbs. MUST NOT look like matcha or strong green.
- ALL PAGES (cover + content): a gentle CURVED WAVE shape along the bottom edge — a soft, organic curve in cool sage-green (#8FA89A to #A0B8AA). The wave MUST have a COOL BLUE-GREEN tone (like the approved cover page), NOT matcha or olive.
- Content pages do NOT have leaf decorations — only the bottom wave.
- NO cartoon plants, NO heavy floral illustrations, NO realistic photos of plants.
- Watercolor-style only — soft, translucent, hand-painted feel.
- LESS IS MORE — decorations should be barely noticeable, like a whisper of nature. Keep it clean and minimal.

TEXT SPACING (CRITICAL FOR CONTENT PAGES):
- Generous line spacing between bullet points — each line should breathe with ample whitespace
- 3-line lists should be evenly distributed across the vertical center with wide gaps
- Text should feel spacious and airy, never cramped
- LEFT-ALIGNED text on content pages

MOOD: Like a premium coastal spa brochure — cool, calming, refreshing. The mint-green background has a COOL BLUE undertone like sea glass or eucalyptus. NEVER warm, NEVER yellow-toned, NEVER matcha-like. Think: cool ocean breeze through mint leavCRITICAL REMINDERS FOR ALL PAGES:
1. Background MUST be the same soft gradient on EVERY page (cover, content, pricing, ending). NEVER use a flat/solid color.
2. Background is primarily WHITE with a whisper of cool mint. NOT a green slide — a WHITE slide with green accents.
3. The bottom wave decoration MUST be cool blue-green (#8FA89A), NOT matcha/olive.
4. Keywords: 爵やかさ・清潔感・安らぎ (freshness, cleanliness, serenity).
```

### テーマ3 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSで実装する。

```
BG_COLOR: #EFF5F1
BG_GRADIENT: radial-gradient(ellipse at 50% 40%, #FAFCFB 0%, #F0F6F2 50%, #EAF2EE 100%)
BG_GRADIENT_DARK: linear-gradient(135deg, #2D5016 0%, #1B5E20 50%, #3A7A3A 100%)
TITLE_GRADIENT_CSS: background: linear-gradient(135deg, #2D5016, #1B5E20, #3A7A3A); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
TITLE_COLOR: #2D5016
SUBTITLE_COLOR: #4A6A3A
TEXT_COLOR: #3A4A3A
BULLET_COLOR: #4A8A50
BULLET_CHAR: —
BANNER_BG: linear-gradient(90deg, #A8C8A0, #4A8A50, #2D5016)
BANNER_BG_WIDE: linear-gradient(90deg, #A8C8A0, #4A8A50, #2D5016, #4A8A50, #A8C8A0)
RULE_COLOR: rgba(74, 138, 80, 0.3)
LINE_COLOR: linear-gradient(90deg, #4A8A50, #2D5016)
PRICE_COLOR: #B8960B
```

---
【装飾 — 表紙（cover）用】
下部の波＋極薄い葉シルエット（CSSのみ）。

```html
<!-- 下部の波装飾 -->
<div style="position:absolute;bottom:0;left:0;width:1280px;height:90px;background:linear-gradient(180deg,transparent 0%,rgba(143,168,154,0.5) 100%);border-radius:60% 60% 0 0 / 40% 40% 0 0;z-index:1;pointer-events:none;"></div>

<!-- 左上極薄い葉シルエット -->
<div style="position:absolute;top:-20px;left:-20px;width:200px;height:200px;background:radial-gradient(ellipse at 30% 30%,rgba(184,200,192,0.20) 0%,transparent 70%);z-index:0;pointer-events:none;"></div>

<!-- 右下極薄い葉シルエット -->
<div style="position:absolute;bottom:60px;right:-20px;width:180px;height:180px;background:radial-gradient(ellipse at 70% 70%,rgba(184,200,192,0.18) 0%,transparent 70%);z-index:0;pointer-events:none;"></div>
```

---
【装飾 — コンテンツページ用】
下部の波のみ（葉シルエットなし）。

```html
<!-- 下部の波装飾 -->
<div style="position:absolute;bottom:0;left:0;width:1280px;height:80px;background:linear-gradient(180deg,transparent 0%,rgba(143,168,154,0.45) 100%);border-radius:60% 60% 0 0 / 40% 40% 0 0;z-index:1;pointer-events:none;"></div>
```

---

## テーマ4: ジオメトリック（Geometric）

**テーマID**: `geometric`
**リファレンス画像**: `templates/themes/theme_04_geometric/`

```
=== THEME OVERRIDE: GEOMETRIC ===

STYLE DIRECTION: UNISEX, MODERN, INTELLECTUAL. This theme is gender-neutral — suitable for both men and women. Think Apple keynote or Google I/O presentation. NOT feminine, NOT soft, NOT romantic. Sharp, clean, structured.

TYPOGRAPHY (CRITICAL — OVERRIDES DEFAULT):
- COVER PAGE ONLY: Japanese serif (Mincho) typeface for title and subtitle — sharp, modern, with clear bone structure (NOT thin/wispy, NOT heavy/bold — REGULAR weight with crisp edges)
- CONTENT PAGES (2nd page onward): Japanese Gothic (sans-serif) typeface — REGULAR weight. Clean and readable. NOT bold/heavy, but also NOT ultra-thin/wispy. Think of a professional tech presentation — clear, neutral, modern.
- Heading banner text: white Gothic sans-serif (regular weight)
- Body text: charcoal gray (#3A3A4A) Gothic sans-serif (regular weight)
- Title text (cover ONLY): blue-to-purple-to-pink gradient Mincho serif
- CRITICAL: Font weight must be IDENTICAL across ALL content pages. NEVER vary the thickness from page to page.

BACKGROUND (CRITICAL — MATCH REFERENCE IMAGE EXACTLY):
- Base: almost pure white (#FFFFFF) with a very subtle cool lavender-blue tint (#F0F0F8). The background should look 90-95% white with a cool, crisp undertone.
- GEOMETRIC LINE DECORATIONS: Very faint, sharp straight lines that SPAN THE ENTIRE SLIDE — like a watermark or frosted glass etching.
  - Line color: barely visible pale gray-lavender, only slightly darker than the white background. Like a watermark printed on white paper.
  - Line thickness: thin but CRISP — equivalent to 1-2px. Sharp edges, NOT soft or blurred.
  - Pattern: LARGE-SCALE intersecting diagonal lines that cross the ENTIRE slide from corner to corner. These lines form large diamond and triangle shapes across the full background — like a geometric crystal structure or faceted glass.
  - The lines are NOT confined to one corner. They span the full width and height of the slide, creating a subtle all-over geometric texture.
  - On the cover page, lines may appear more concentrated in the upper-right area, but on content pages they spread across the entire background.
  - Lines must look like a WATERMARK or FROSTED GLASS ETCHING — extremely subtle, almost invisible at first glance, but creating a sophisticated geometric texture upon close inspection.
- CRITICAL: The background should feel clean and modern. The lines are a full-slide geometric texture, NOT a small decorative element in one corner.

COLOR PALETTE:
- Background: white to cool lavender-blue (#FFFFFF to #F0F0F8)
- Primary text: charcoal gray (#3A3A4A)
- Title text (cover/section ONLY): blue-to-purple-to-pink gradient (#4A7AD9 → #7A4ABF → #C04A8A). Mincho serif. The gradient flows LEFT to RIGHT — blue on the left, transitioning through purple to pink/magenta on the right.
- Subtitle text: muted lavender-gray (#8A8A9A)
- Accent: warm gold (#B8960B) for price highlights ONLY
- Heading banner (small, コンセプト style): blue-to-purple-to-pink gradient (#4A7AD9 → #7A4ABF → #C04A8A) with white text, compact rectangle at top-left
- Heading banner (large, この講座から得られる未来 style): wider blue-to-purple-to-pink gradient band, centered white text
- Bullet icons: none (text only, or subtle dash)

DECORATIVE ELEMENTS (CRITICAL — MATCH REFERENCE IMAGE EXACTLY):
- BOTTOM FOOTER BAND: A gentle, smooth gradient band hugging the very bottom edge of the slide.
  - The band uses the blue-to-purple-to-pink gradient (#4A7AD9 → #7A4ABF → #C04A8A). Blue on the left, transitioning to purple in the center, to pink on the right.
  - Band height: approximately 3-5% of slide height. It is a SLIM, FLAT footer strip.
  - The top edge of the band has a very gentle curve — like a distant hill silhouette or a very gentle arc. NOT a dramatic wave, NOT an S-curve, NOT a ribbon. Just a subtle, smooth, barely-curved top edge.
  - The band fades softly into the background at its top edge (soft gradient fade, not a hard line).
  - Think of it as a FOOTER GRADIENT STRIP that sits at the bottom of the slide, similar to a gentle horizon line.
  - NEVER a dramatic wave or undulating ribbon. NEVER multiple overlapping curves.
  - The footer band must look IDENTICAL in thickness and style on EVERY page.
- BACKGROUND LINES: as described above — faint, sharp, spanning the entire slide as a geometric watermark texture
- NO neon glow, NO 3D effects, NO heavy patterns, NO soft/blurred decorations
- LESS IS MORE — the subtle footer band and faint geometric watermark lines are the ONLY decorations

CRITICAL REMINDERS FOR ALL PAGES:
1. This is a UNISEX, GENDER-NEUTRAL design. NOT feminine, NOT soft. Sharp, modern, intellectual.
2. Background geometric lines must SPAN THE ENTIRE SLIDE as a watermark-like texture. They are NOT confined to one corner. They form large diamond/triangle shapes across the full background.
3. Background lines must be BARELY VISIBLE — like a watermark on white paper. If they look prominent or dark, they are TOO STRONG.
4. Bottom footer band must be a GENTLE, SLIM gradient strip (3-5% of slide height) with a barely-curved top edge. NOT a dramatic wave, NOT a ribbon, NOT an S-curve.
5. Font weight on content pages must be REGULAR (not bold, not ultra-thin). Consistent across all pages.
6. Always include the theme reference image (cover_approved.png) in references to match the exact decoration style.

TEXT SPACING (CRITICAL FOR CONTENT PAGES):
- Generous line spacing between bullet points — each line should breathe with ample whitespace
- 3-line lists should be evenly distributed across the vertical center with wide gaps
- Text should feel spacious and clean, never cramped
- LEFT-ALIGNED text on content pages

MOOD: Like a cutting-edge tech company keynote (Apple, Google, Tesla) — structured, forward-thinking, intellectual. The blue-purple-pink gradient gives it energy and modernity, while the geometric background lines add sophistication. Clean, sharp, confident. Gender-neutral and professional. NOT feminine, NOT romantic, NOT soft.
```

### テーマ4 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSで実装する。

```
BG_COLOR: #F8F8FC
BG_GRADIENT: radial-gradient(ellipse at 50% 40%, #FFFFFF 0%, #F5F5FB 50%, #F0F0F8 100%)
BG_GRADIENT_DARK: linear-gradient(135deg, #4A7AD9 0%, #7A4ABF 50%, #C04A8A 100%)
TITLE_GRADIENT_CSS: background: linear-gradient(90deg, #4A7AD9, #7A4ABF, #C04A8A); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
TITLE_COLOR: #7A4ABF
SUBTITLE_COLOR: #8A8A9A
TEXT_COLOR: #3A3A4A
BULLET_COLOR: #7A4ABF
BULLET_CHAR: —
BANNER_BG: linear-gradient(90deg, #4A7AD9, #7A4ABF, #C04A8A)
BANNER_BG_WIDE: linear-gradient(90deg, #4A7AD9, #7A4ABF, #C04A8A)
RULE_COLOR: rgba(122, 74, 191, 0.3)
LINE_COLOR: linear-gradient(90deg, #4A7AD9, #7A4ABF, #C04A8A)
PRICE_COLOR: #B8960B
```

---
【装飾 — 全ページ共通】
背景に極薄い幾何学線（ウォーターマーク風）、下部にスリムなグラデーション帯。

```html
<!-- 背景幾何学線（ウォーターマーク風） -->
<div style="position:absolute;top:0;left:0;width:1280px;height:720px;z-index:0;pointer-events:none;overflow:hidden;">
  <div style="position:absolute;top:-100px;left:-100px;width:1480px;height:920px;background:repeating-linear-gradient(45deg,rgba(122,74,191,0.04) 0px,rgba(122,74,191,0.04) 1px,transparent 1px,transparent 80px),repeating-linear-gradient(-45deg,rgba(74,122,217,0.04) 0px,rgba(74,122,217,0.04) 1px,transparent 1px,transparent 80px);"></div>
</div>

<!-- 下部グラデーション帯 -->
<div style="position:absolute;bottom:0;left:0;width:1280px;height:36px;background:linear-gradient(90deg,#4A7AD9,#7A4ABF,#C04A8A);border-radius:8px 8px 0 0;z-index:1;pointer-events:none;"></div>
```

---

## テーマ5: ソフトベージュ（Soft Beige）

**テーマID**: `soft_beige`
**リファレンス画像**: `templates/themes/theme_05_soft_beige/`

```
=== THEME OVERRIDE: SOFT BEIGE ===

CRITICAL INSTRUCTION: You MUST replicate the EXACT visual style of the provided reference images.
Copy the reference images' background texture, decoration style, color tones, and overall atmosphere as closely as possible.
The reference images are the single source of truth for this theme's visual identity.

TYPOGRAPHY:
- ALL text: feminine Japanese serif (Mincho) typeface — elegant, thin strokes
- NEVER use Gothic (sans-serif) typeface anywhere
- Body text: soft charcoal-brown (#5A4A44) Mincho serif
- Title text (cover/section): warm peach-to-brown gradient (#D4A870 → #B87860 → #C08878) Mincho serif
- Subtitle text: light warm gray (#A09888)
- Heading banner text: white Mincho serif on soft gradient banner

BACKGROUND:
- Cream-white (#FFFCF8) as the base color
- The background should feel like warm, soft morning light on cream-colored paper

COLOR PALETTE:
- Background: cream-white (#FFFCF8)
- Body text: soft charcoal-brown (#5A4A44)
- Title text: warm peach-to-brown gradient
- Subtitle: warm gray (#A09888)
- Price accent: warm gold (#C8A830)
- Heading banner: soft peach-beige-to-dusty-pink gradient (#D8B8A0 → #CCA0A0) with white text

DECORATIVE ELEMENTS (COPY REFERENCE IMAGES EXACTLY):

1. ORGANIC BLOB SHAPES:
   - Soft, organic, rounded blob shapes placed at corners of the slide
   - Edges must be HEAVILY BLURRED / SOFT-FOCUS — blobs must FADE and DISSOLVE into the cream background
   - NO sharp edges, NO crisp outlines — think of soft light glowing through frosted glass
   - Colors: Pale Yellow, Ash Beige, Pale Salmon — all in very soft, muted pale tones
   - Blobs should overlap slightly and layer on top of each other for depth

2. SUBTLE DOT PATTERN (HALFTONE):
   - In the BOTTOM-RIGHT area, include a faint halftone dot pattern (small evenly-spaced dots)
   - The dots should be in a pale warm yellow or gold tone, very faint
   - This is a signature element of this theme — always include it

3. THIN GRAY CURVED LINES:
   - 1-2 very thin, delicate curved lines (like fine thread) placed near blob edges
   - Color: very light gray (#D8D8D8), extremely thin hairline
   - Lines should feel like gentle, flowing curves — not geometric
   - Lines must NEVER cross or touch text areas

4. TEXT OVERLAP PROHIBITION (ABSOLUTE RULE):
   - Decorations MUST NEVER overlap, touch, or come close to ANY text
   - Minimum clear margin of 20% between any decoration and any text
   - Text readability is the #1 priority

5. PLACEMENT:
   - COVER PAGE: blobs at TOP-LEFT (yellow/beige), TOP-RIGHT (salmon/beige), BOTTOM-RIGHT (salmon + dot pattern). Keep center clear for title.
   - CONTENT PAGES: smaller, more subtle blobs. Mainly BOTTOM-RIGHT corner with dot pattern. 1 small blob at TOP-LEFT or TOP-RIGHT. Central area must be clean for text.

TEXT SPACING:
- Generous line spacing, airy and spacious layout
- LEFT-ALIGNED text on content pages

MOOD:
- Bright, soft, and reassuring — like a warm wellness space bathed in soft morning light
- Clean, inviting, feminine — high-end lifestyle magazine feel
- The overall atmosphere should feel like looking through a soft-focus lens
- NEVER dark, NEVER heavy, NEVER muddy, NEVER busy
```

### テーマ5 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSの `radial-gradient` でブロブを実装する。

```
BG_COLOR: #FFFCF8
BG_GRADIENT: #FFFCF8
TITLE_GRADIENT: linear-gradient(135deg, #D4A870, #B87860, #C08878)
TITLE_GRADIENT_CSS: background: linear-gradient(135deg, #D4A870, #B87860, #C08878); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
SUBTITLE_COLOR: #A09888
TEXT_COLOR: #5A4A44
BULLET_COLOR: #D4A870
BULLET_CHAR: ◆
BANNER_BG: linear-gradient(90deg, #D8B8A0, #CCA0A0)
RULE_COLOR: rgba(212, 168, 112, 0.3)
LINE_COLOR: linear-gradient(90deg, #D4A870, #B87860)
```

---
【ブロブ装飾 — 表紙（cover）用】
以下の3つのdivをposition:absoluteで配置する（外部画像不要）。

```html
<!-- 左上ブロブ：クリームイエロー -->
<div style="position:absolute;top:-100px;left:-100px;width:420px;height:380px;background:radial-gradient(ellipse at center,rgba(245,230,195,0.65) 0%,rgba(245,230,195,0.30) 50%,transparent 75%);z-index:0;pointer-events:none;"></div>

<!-- 右上ブロブ：サーモンピンク -->
<div style="position:absolute;top:-60px;right:-60px;width:300px;height:300px;background:radial-gradient(ellipse at center,rgba(242,196,172,0.60) 0%,rgba(242,196,172,0.28) 50%,transparent 75%);z-index:0;pointer-events:none;"></div>

<!-- 右下ブロブ：ピーチサーモン -->
<div style="position:absolute;bottom:-100px;right:-100px;width:420px;height:400px;background:radial-gradient(ellipse at center,rgba(240,190,165,0.65) 0%,rgba(240,190,165,0.30) 50%,transparent 75%);z-index:0;pointer-events:none;"></div>
```

---
【ブロブ装飾 — コンテンツページ用（bullet-list, phase-card, feature-card等）】

```html
<!-- 左上ブロブ：控えめなクリームイエロー -->
<div style="position:absolute;top:-80px;left:-80px;width:280px;height:260px;background:radial-gradient(ellipse at center,rgba(245,230,195,0.45) 0%,rgba(245,230,195,0.20) 50%,transparent 75%);z-index:0;pointer-events:none;"></div>

<!-- 右下ブロブ：控えめなピーチサーモン -->
<div style="position:absolute;bottom:-80px;right:-80px;width:280px;height:260px;background:radial-gradient(ellipse at center,rgba(240,190,165,0.45) 0%,rgba(240,190,165,0.20) 50%,transparent 75%);z-index:0;pointer-events:none;"></div>
```

**注意**: ゴールドドット装飾は使用しない（ユーザー確認済みで削除）。

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

---

## テーマ6: ナチュラルピンク（Natural Pink）

**テーマID**: `natural_pink`
**リファレンス画像**: `templates/themes/theme_06_natural_pink/`

```
=== THEME OVERRIDE: NATURAL PINK ===

CRITICAL INSTRUCTION: You MUST replicate the EXACT visual style of the provided reference images.
Copy the reference images' background texture, decoration style, color tones, and overall atmosphere as closely as possible.
The reference images are the single source of truth for this theme's visual identity.

TYPOGRAPHY:
- ALL text: feminine Japanese serif (Mincho) typeface — elegant, thin strokes
- NEVER use Gothic (sans-serif) typeface anywhere
- Body text: charcoal gray (#4A4A4A) Mincho serif
- Title text (cover/section): rose pink-to-dusty pink gradient (#D4707A → #B86878 → #A85868) Mincho serif
- Subtitle text: warm gray (#9A8A8A)
- Heading banner text: white Mincho serif on soft pink gradient banner
- Title underline: thin horizontal line in rose pink, placed directly below the title text

BACKGROUND:
- PURE WHITE (#FFFFFF) as the base color for ALL pages
- The background should feel bright, clean, and airy — like a luxury bridal salon
- Content pages may have a very faint pink warmth (#FFFBFC) but should read as essentially white

COLOR PALETTE:
- Background: pure white (#FFFFFF)
- Body text: charcoal gray (#4A4A4A)
- Title text: rose pink-to-dusty pink gradient (#D4707A → #B86878)
- Subtitle: warm gray (#9A8A8A)
- Price accent: warm gold gradient band (#C8A850 → #B89840) — same style as other themes
- Heading banner (small, コンセプト style): soft pink gradient (#E0A0B0 → #D090A0) with white text, compact rectangle at top-left
- Heading banner (large, この講座から得られる未来 style): wider soft pink gradient band across upper area, centered white text
- Accent labels (対象:, 期間:, 提供内容): rose pink (#C06878)
- Separator lines: very thin pink-to-lavender gradient lines

DECORATIVE ELEMENTS (COPY REFERENCE IMAGES EXACTLY):

1. WATERCOLOR PINK BLUSH CLOUDS:
   - Soft, dreamy watercolor-style pink blush shapes placed at corners of the slide
   - These are NOT solid blobs — they are translucent, airy watercolor washes that fade into the white background
   - Colors: soft rose pink (#F0B0C0), pale coral pink (#F0C0C8), dusty pink (#E8A8B8)
   - Edges are completely diffused — like watercolor paint dropped on wet paper, bleeding outward
   - COVER PAGE: larger blush clouds at TOP-LEFT and BOTTOM-RIGHT (diagonal placement)
   - CONTENT PAGES: smaller, more subtle blush clouds. Mainly corners, keeping center clean for text.
   - The watercolor effect should look hand-painted, organic, and soft — NOT digital, NOT flat, NOT sharp-edged

2. GOLD FRAME LINES (SIGNATURE ELEMENT):
   - Two thin vertical gold lines running along the LEFT and RIGHT edges of the slide
   - Color: warm gold (#C8A850 → #D4B860) — a refined, muted gold, NOT bright/flashy
   - Line thickness: very thin (1-2px equivalent), like a fine gold thread
   - Lines run from top to bottom of the slide, positioned approximately 3-5% from each edge
   - These gold frame lines appear on EVERY page as consistent branding
   - The gold lines give the slide a "framed" feeling, like a premium certificate or invitation

3. INK SPLASH DOTS (SUBTLE ACCENT):
   - Tiny, scattered ink-splash dots near the watercolor blush areas (especially top-left)
   - Colors: muted gray (#A0A0A0), dark sage green (#607060), dusty pink (#C0A0A8)
   - Very small (2-5px equivalent), randomly scattered, like paint spatters
   - Only 5-10 dots total per slide — NOT dense, NOT a pattern
   - These add an organic, hand-crafted feel to the watercolor aesthetic

4. TEXT OVERLAP PROHIBITION (ABSOLUTE RULE):
   - Decorations MUST NEVER overlap, touch, or come close to ANY text
   - Minimum clear margin of 15% between any decoration and any text
   - Text readability is the #1 priority
   - The center of the slide must remain clean and open for text

5. PLACEMENT SUMMARY:
   - COVER PAGE: watercolor blush at TOP-LEFT (larger) + BOTTOM-RIGHT (larger). Gold frame lines on both sides. Ink dots near top-left blush. Center clean for title.
   - CONTENT PAGES: watercolor blush at corners (smaller, more subtle). Gold frame lines on both sides. Minimal ink dots. Central area clean for text.
   - PRICING PAGE: same as content but with gold gradient price band on left side

TEXT STYLE (CRITICAL — FEMININE ELEGANCE RULE):
- Body text MUST use THIN / REGULAR weight only — NEVER Bold, Semi-Bold, or Heavy
- Body text size: approximately 60-65% of the header banner text size — modest and delicate, NOT large or commanding
- The text should feel like it is "whispering" — light, airy, graceful
- Think of a luxury beauty brand brochure: understated, refined, with lots of breathing room
- Check mark (✓) icons: soft rose pink, same thin weight as body text

TEXT SPACING & WHITE SPACE (CRITICAL — BREATHABLE LAYOUT):
- Generous line spacing, airy and spacious layout
- LEFT-ALIGNED text on content pages
- Each bullet point should breathe with ample whitespace
- Left margin: 20% from left edge (wider than standard)
- Right margin: 25% from right edge (wider than standard)
- Bottom 25% of the slide should remain EMPTY white space (decorations only)
- The slide should feel SPACIOUS and CALMING — never crowded or text-heavy
- Prioritize white space over information density

MOOD:
- Soft, romantic, and feminine — like a luxury bridal salon or high-end beauty magazine
- Bright and airy with a warm pink glow — inviting and reassuring
- The watercolor elements give it an artistic, hand-crafted quality
- The gold frame lines add a touch of premium elegance
- Overall: warm, welcoming, beautiful — makes the viewer feel special and cared for
- NEVER dark, NEVER heavy, NEVER harsh, NEVER cold
- Think: cherry blossom petals, silk ribbons, morning light through pink curtains
```

### テーマ6 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSで実装する。

```
BG_COLOR: #FFFBFC
BG_GRADIENT: radial-gradient(ellipse at 50% 40%, #FFFFFF 0%, #FFF5F8 50%, #FFF0F4 100%)
BG_GRADIENT_DARK: linear-gradient(135deg, #D4707A 0%, #B86878 100%)
TITLE_GRADIENT_CSS: background: linear-gradient(90deg, #D4707A, #B86878); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
TITLE_COLOR: #D4707A
SUBTITLE_COLOR: #9A8A8A
TEXT_COLOR: #4A4A4A
BULLET_COLOR: #D4707A
BULLET_CHAR: —
BANNER_BG: linear-gradient(90deg, #E0A0B0, #D090A0)
BANNER_BG_WIDE: linear-gradient(90deg, #E0A0B0, #D090A0, #E0A0B0)
RULE_COLOR: rgba(212, 112, 122, 0.3)
LINE_COLOR: linear-gradient(90deg, #D4707A, #B86878)
PRICE_COLOR: #C8A850
```

---
【装飾 — 表紙（cover）用】
左右両端に細いゴールド縦線、左上にピンクのグロー。

```html
<!-- 左端ゴールド縦線 -->
<div style="position:absolute;top:0;left:20px;width:1px;height:100%;background:linear-gradient(180deg,rgba(200,168,80,0.6) 0%,rgba(200,168,80,0.3) 100%);z-index:0;pointer-events:none;"></div>

<!-- 右端ゴールド縦線 -->
<div style="position:absolute;top:0;right:20px;width:1px;height:100%;background:linear-gradient(180deg,rgba(200,168,80,0.6) 0%,rgba(200,168,80,0.3) 100%);z-index:0;pointer-events:none;"></div>

<!-- 左上ピンクグロー -->
<div style="position:absolute;top:-40px;left:-40px;width:280px;height:280px;background:radial-gradient(ellipse at 30% 30%,rgba(240,176,192,0.35) 0%,transparent 70%);z-index:0;pointer-events:none;"></div>

<!-- 右下ピンクグロー -->
<div style="position:absolute;bottom:-40px;right:-40px;width:260px;height:260px;background:radial-gradient(ellipse at 70% 70%,rgba(240,176,192,0.30) 0%,transparent 70%);z-index:0;pointer-events:none;"></div>
```

---
【装飾 — コンテンツページ用】
左右ゴールド縦線＋左上に控えめのピンクグロー。

```html
<!-- 左端ゴールド縦線 -->
<div style="position:absolute;top:0;left:20px;width:1px;height:100%;background:linear-gradient(180deg,rgba(200,168,80,0.5) 0%,rgba(200,168,80,0.25) 100%);z-index:0;pointer-events:none;"></div>

<!-- 右端ゴールド縦線 -->
<div style="position:absolute;top:0;right:20px;width:1px;height:100%;background:linear-gradient(180deg,rgba(200,168,80,0.5) 0%,rgba(200,168,80,0.25) 100%);z-index:0;pointer-events:none;"></div>

<!-- 左上控えめピンクグロー -->
<div style="position:absolute;top:-20px;left:-20px;width:180px;height:180px;background:radial-gradient(ellipse at 30% 30%,rgba(240,176,192,0.22) 0%,transparent 70%);z-index:0;pointer-events:none;"></div>
```

---

## テーマ7: ネイビーゴールド（Navy Gold）

**テーマID**: `navy_gold`
**向いているジャンル**: 男性向け、ビジネス系、コンサルティング、投資、経営者向け
**参照画像**: `templates/themes/theme_07_navy_gold/`

```
=== THEME OVERRIDE: NAVY GOLD ===

CRITICAL: You MUST use the provided theme reference images as your PRIMARY style guide.
Copy the exact color tones, textures, gradients, and atmosphere from the reference images.
The reference images are the ABSOLUTE AUTHORITY for this theme's visual style.

COLOR PALETTE:
- Background (COVER): Deep navy blue gradient — top-left lighter (#818FA7), bottom-right darker (#0C1856). Linear gradient from top-left to bottom-right.
- Background (CONTENT): Light silver-gray gradient at top 70% (#C8CDD8 to #D8DCE5), transitioning to navy band at bottom 15% (#1A2550). Clean and professional.
- Title text (COVER): Pure white (#FFFFFF), large serif font, elegant and commanding
- Subtitle text (COVER): White (#FFFFFF), smaller, clean sans-serif
- Body text (CONTENT): Deep navy (#1A2550 to #1E2D5A), Gothic/sans-serif font — NOT too bold, medium weight
- Header banner: Deep navy gradient (#1A2550 to #2A3A6A), rectangular, positioned top-left
- Banner text: White (#FFFFFF)
- Accent: Gold (#B8953F to #D4AF5A) — used ONLY for frame lines and price band

DECORATIVE ELEMENTS:
- COVER PAGE:
  - Full-bleed navy gradient background (center lighter, edges darker)
  - Gold diagonal frame lines: thin elegant lines running from corners inward, creating a geometric frame effect
  - Lines are THIN (1-2px equivalent), NOT thick or heavy
  - NO watercolor, NO organic shapes — purely geometric and sharp
  - Thin white horizontal line below title (centered, ~40% width)

- CONTENT PAGES:
  - Top 70-75%: Light silver-gray gradient background (cool-toned, professional)
  - Thin horizontal gold line separating gray area from navy band (~1px)
  - Bottom 15-20%: Solid deep navy band (#1A2550)
  - Very thin gold accent line at the very bottom edge
  - Header banner: deep navy rectangle, top-left, white text
  - NO watercolor, NO organic shapes, NO dots — clean corporate aesthetic

- PRICING PAGE:
  - Same top silver-gray + bottom navy band structure as content pages
  - Left column: product name + gold gradient price band (horizontal strip behind price text)
  - Vertical divider line between columns (thin, navy or gold)
  - Right column: details in navy text on silver-gray background

TEXT STYLE (MASCULINE BUSINESS RULE):
- Body text: Gothic/sans-serif font, MEDIUM weight — NOT Bold, NOT Heavy, NOT too thin
- Body text should feel authoritative but not aggressive — professional and clear
- Think of a premium business consulting firm's presentation
- Font weight should match the reference images exactly — clean and readable

TEXT SPACING:
- Generous line spacing, structured and organized
- LEFT-ALIGNED text on content pages
- Professional spacing — not too tight, not too loose
- Clean grid-like organization

MOOD:
- Authoritative, trustworthy, premium — like a top-tier consulting firm or investment bank presentation
- The navy conveys depth and reliability
- The gold accents convey exclusivity and premium value
- The silver-gray content background keeps readability high while maintaining sophistication
- Overall: powerful, confident, professional — makes the viewer feel they're dealing with a serious, high-value offering
- NEVER playful, NEVER cute, NEVER casual, NEVER colorful
- Think: executive boardroom, luxury watch advertisement, private banking brochure
===
```

### テーマ7 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSで実装する。

**フォント**: Noto Sans JP（weight: 300;400;500;700）— コンテンツページのみゴシック体。表紙はNoto Serif JP。

```
BG_COLOR: #C8CDD8
BG_GRADIENT: linear-gradient(135deg, #818FA7 0%, #0C1856 100%)
BG_GRADIENT_DARK: linear-gradient(135deg, #1A2550 0%, #2A3A6A 100%)
BG_GRADIENT_CONTENT: linear-gradient(135deg, #ECEEF4 0%, #DDE0E8 45%, #C8CDD8 93%, #1A2550 93%)
TITLE_GRADIENT_CSS: color: #FFFFFF;
TITLE_COLOR: #FFFFFF
SUBTITLE_COLOR: rgba(255,255,255,0.85)
TEXT_COLOR: #1A2550
BULLET_COLOR: linear-gradient(90deg, #8A6A20, #B8953F, #D4AF5A)
BULLET_CHAR: ■
BANNER_BG: linear-gradient(90deg, #0D1A3A, #1A2550, #2A3A6A, #1E2E5A)
BANNER_BG_WIDE: linear-gradient(90deg, #0D1A3A, #1A2550, #2A3A6A, #1A2550, #0D1A3A)
BANNER_FONT_SIZE: 26px
BANNER_PADDING: 12px 36px
RULE_COLOR: rgba(212, 175, 90, 0.6)
LINE_COLOR: linear-gradient(90deg, #8A6A20, #B8953F, #D4AF5A, #C8A84E, #B8953F)
PRICE_COLOR: linear-gradient(90deg, #B8953F, #D4AF5A, #C8A84E)
GOLD_TEXT_GRADIENT: background:linear-gradient(90deg,#8A6A20,#B8953F,#D4AF5A);-webkit-background-clip:text;-webkit-text-fill-color:transparent;

【フォントサイズ確定値 — コンテンツページ】
BANNER_TEXT: 26px / font-weight:700
BULLET_ICON: 40px
BULLET_TEXT: 38px / font-weight:500
PROFILE_TITLE: 48px / Noto Serif JP
PROFILE_SUBTITLE: 20px / font-weight:500
PROFILE_BULLET: 26px
PHASE_LABEL: 24px / font-weight:700
PHASE_TITLE: 36px / Noto Serif JP
PHASE_BODY: 26px / font-weight:500 / line-height:1.5
PRICING_PLAN_NAME: 52px / Noto Serif JP
PRICING_PRICE: 60px / Noto Serif JP
PRICING_ITEM: 24px

【改行ポリシー】
- 説明文に<br>は原則入れない。ブラウザの自動折り返しに任せる。
- コンテンツが多すぎて枠からはみ出る場合は、改行ではなく「テキスト量を短くまとめる」で対応する。
- フェーズカードの説明文は最大60字以内を目安に。
```

---
【装飾 — 表紙（cover）用】
背景はネイビーグラデーション（radial）、四隅にゴールドの方向線。フォントはNoto Serif JP。

```html
<!-- 左上ゴールド方向線 -->
<div style="position:absolute;top:0;left:0;width:200px;height:200px;z-index:0;pointer-events:none;">
  <div style="position:absolute;top:30px;left:30px;width:120px;height:1px;background:linear-gradient(90deg,rgba(212,175,90,0.8),transparent);transform:rotate(45deg);transform-origin:0 0;"></div>
  <div style="position:absolute;top:50px;left:50px;width:90px;height:1px;background:linear-gradient(90deg,rgba(212,175,90,0.5),transparent);transform:rotate(45deg);transform-origin:0 0;"></div>
</div>

<!-- 右下ゴールド方向線 -->
<div style="position:absolute;bottom:0;right:0;width:200px;height:200px;z-index:0;pointer-events:none;">
  <div style="position:absolute;bottom:30px;right:30px;width:120px;height:1px;background:linear-gradient(270deg,rgba(212,175,90,0.8),transparent);transform:rotate(45deg);transform-origin:100% 0;"></div>
  <div style="position:absolute;bottom:50px;right:50px;width:90px;height:1px;background:linear-gradient(270deg,rgba(212,175,90,0.5),transparent);transform:rotate(45deg);transform-origin:100% 0;"></div>
</div>
```

---
【装飾 — コンテンツページ用】
背景は左上から右下への対角グラデーション（左上: 明るいシルバーホワイト #ECEEF4 → 右下: グレーブルー #C8CDD8）、下7%ネイビー帯（48px）。ゴールドラインは帯の内側（bottom:12px）。
コンテンツエリアは必ず下部帯（48px）を避けて配置すること。フォントはNoto Sans JP（weight:500）。

```html
<!-- 下部ネイビーグラデーション帯（height:48px） -->
<div style="position:absolute;bottom:0;left:0;width:100%;height:48px;background:linear-gradient(90deg,#0D1A3A,#1A2550,#2A3A6A,#1A2550,#0D1A3A);z-index:0;pointer-events:none;"></div>

<!-- シャンパンゴールド区切り線（帯の内側 bottom:12px） -->
<div style="position:absolute;bottom:12px;left:0;width:100%;height:1px;background:linear-gradient(90deg,transparent,#8A6A20,#B8953F,#D4AF5A,#C8A84E,#B8953F,#8A6A20,transparent);z-index:0;pointer-events:none;"></div>
```

---
【コンテンツページ共通ヘッダー（バナー＋ゴールドライン）】
全コンテンツページの上部に必ず配置する。

```html
<!-- 左上バナー -->
<div style="position:relative;z-index:1;margin-top:44px;margin-left:60px;display:inline-block;">
  <div style="background:linear-gradient(90deg,#0D1A3A,#1A2550,#2A3A6A,#1E2E5A);padding:12px 36px;">
    <span style="font-family:'Noto Sans JP',sans-serif;font-size:22px;font-weight:700;color:#FFFFFF;letter-spacing:0.08em;">【見出しテキスト】</span>
  </div>
</div>

<!-- シャンパンゴールド横線 -->
<div style="position:relative;z-index:1;margin:0 60px;height:1.5px;background:linear-gradient(90deg,#8A6A20,#B8953F,#D4AF5A,#C8A84E,#B8953F,rgba(184,149,63,0.2));margin-top:14px;"></div>
```

---

## テーマ8: グレーゴールド（Gray Gold）

**テーマID**: `gray_gold`
**向いているジャンル**: 男性向け、ビジネス系、コンサルティング、経営者向け、投資
**参照画像**: `templates/themes/theme_08_gray_gold/`

```
=== THEME OVERRIDE: GRAY GOLD ===

CRITICAL: You MUST use the provided theme reference images as your PRIMARY style guide.
Copy the exact color tones, textures, gradients, and atmosphere from the reference images.
The reference images are the ABSOLUTE AUTHORITY for this theme's visual style.

COLOR PALETTE:
- Background (COVER): Gray gradient — top-left lighter (#9D9B9B), bottom-right darker (#4A4949). Linear gradient from top-left to bottom-right. Neutral, achromatic, sophisticated.
- Background (CONTENT): Light gray gradient at top 70-75% (#D8D8D8 to #E5E5E5), very pale and clean. Transitioning to dark charcoal-gray band at bottom 15-20% (#3A3A3A to #4A4A4A).
- Title text (COVER): Champagne gold gradient (#F8E6C8, #DDBE7B, #FFE9AC, #FDF3D5, #B19549), large serif font, luxurious and commanding. The gold should have a subtle metallic sheen — NOT flat, NOT overly shiny.
- Subtitle text (COVER): Muted warm gray (#8A8080 to #7A7070), smaller, clean sans-serif
- Body text (CONTENT): Dark charcoal (#333333 to #4A4A4A), Gothic/sans-serif font — NOT too bold, medium weight
- Header banner (small): Dark gray gradient (#3A3A3A to #5A5A5A), rectangular, positioned top-left
- Header banner (large): Wider dark gray gradient band, centered at top area
- Banner text: White (#FFFFFF)
- Accent: Champagne Gold (#F8E6C8, #DDBE7B, #FFE9AC, #FDF3D5, #B19549) — used ONLY for frame lines, price band, and title underline

DECORATIVE ELEMENTS:
- COVER PAGE:
  - Full-bleed medium gray gradient background (center lighter, edges darker)
  - White right-angle frame lines: thin white lines forming L-shaped corner brackets at TOP-LEFT and BOTTOM-RIGHT corners
  - Top-left: two nested L-shaped lines (like a bracket) pointing inward from the corner
  - Bottom-right: two nested L-shaped lines (like a bracket) pointing inward from the corner — mirror of top-left
  - Lines are THIN (1-2px equivalent), pure white (#FFFFFF), NOT thick or heavy
  - Thin gold horizontal line below the title text (centered, ~40% width)
  - NO diagonal lines, NO watercolor, NO organic shapes — purely geometric and clean
  - The corner brackets give a structured, architectural feel

- CONTENT PAGES:
  - Top 70-75%: Light gray gradient background (neutral, clean)
  - Thin horizontal gold line (#B8953F to #D4AF5A) separating gray area from dark band (~1px)
  - Bottom 15-20%: Solid dark charcoal-gray band (#3A3A3A to #4A4A4A)
  - Very thin gold accent line at the very bottom edge
  - Header banner: dark gray gradient rectangle, top-left (small type) or centered wide band (large type), white text
  - NO watercolor, NO organic shapes, NO dots — clean corporate aesthetic

- PRICING PAGE:
  - Same top light gray + bottom dark gray band structure as content pages
  - Left column: product name + gold gradient price band (horizontal strip behind price text)
  - Vertical divider line between columns (thin, gray or gold)
  - Right column: details in dark charcoal text on light gray background

TEXT STYLE (MASCULINE BUSINESS RULE):
- Body text: Gothic/sans-serif font, MEDIUM weight — NOT Bold, NOT Heavy, NOT too thin
- Body text should feel authoritative but not aggressive — professional and clear
- Think of a premium business consulting firm's presentation
- Font weight should match the reference images exactly — clean and readable

TEXT SPACING:
- Generous line spacing, structured and organized
- LEFT-ALIGNED text on content pages
- Professional spacing — not too tight, not too loose
- Clean grid-like organization

MOOD:
- Sophisticated, understated, premium — like a luxury architecture firm or high-end real estate presentation
- The neutral gray conveys timeless elegance and professionalism
- The gold accents convey exclusivity and premium value without being flashy
- The achromatic palette feels more understated and refined than the Navy Gold theme
- Overall: calm authority, quiet confidence, mature sophistication — makes the viewer feel they're dealing with a serious, established brand
- NEVER playful, NEVER cute, NEVER casual, NEVER colorful
- Think: luxury watch catalog, premium car brochure, private wealth management office
- KEY DIFFERENCE FROM NAVY GOLD: This theme is ACHROMATIC (no blue/color) — all grays + gold. More subtle, more neutral, more universally sophisticated.
===
```

### テーマ8 HTML変数定義（HTMLモード用・確定版）

HTMLモードでスライドを生成する際、以下のCSS変数・HTML要素を使用する。
**装飾方式**: 外部画像不要。純粋なCSSで実装する。

```
BG_COLOR: #D8D8D8
BG_GRADIENT: linear-gradient(135deg, #9D9B9B 0%, #4A4949 100%)
BG_GRADIENT_DARK: linear-gradient(135deg, #3A3A3A 0%, #5A5A5A 100%)
BG_GRADIENT_CONTENT: linear-gradient(180deg, #D8D8D8 0%, #E5E5E5 70%, #3A3A3A 70%)
TITLE_GRADIENT_CSS: background: linear-gradient(90deg, #F8E6C8, #DDBE7B, #FFE9AC, #FDF3D5, #B19549); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;
TITLE_COLOR: #DDBE7B
SUBTITLE_COLOR: rgba(255,255,255,0.75)
TEXT_COLOR: #333333
BULLET_COLOR: #DDBE7B
BULLET_CHAR: ■
BANNER_BG: linear-gradient(90deg, #3A3A3A, #5A5A5A)
BANNER_BG_WIDE: linear-gradient(90deg, #3A3A3A, #5A5A5A, #3A3A3A)
RULE_COLOR: rgba(221, 190, 123, 0.5)
LINE_COLOR: linear-gradient(90deg, #F8E6C8, #DDBE7B, #FFE9AC, #FDF3D5, #B19549)
PRICE_COLOR: #DDBE7B
```

---
【装飾 — 表紙（cover）用】
背景はグレーグラデーション、左上・右下に白のL字ブラケット線。

```html
<!-- 左上白ブラケット線 -->
<div style="position:absolute;top:0;left:0;width:120px;height:120px;z-index:0;pointer-events:none;">
  <div style="position:absolute;top:24px;left:24px;width:70px;height:1px;background:rgba(255,255,255,0.7);"></div>
  <div style="position:absolute;top:24px;left:24px;width:1px;height:70px;background:rgba(255,255,255,0.7);"></div>
  <div style="position:absolute;top:36px;left:36px;width:50px;height:1px;background:rgba(255,255,255,0.4);"></div>
  <div style="position:absolute;top:36px;left:36px;width:1px;height:50px;background:rgba(255,255,255,0.4);"></div>
</div>

<!-- 右下白ブラケット線 -->
<div style="position:absolute;bottom:0;right:0;width:120px;height:120px;z-index:0;pointer-events:none;">
  <div style="position:absolute;bottom:24px;right:24px;width:70px;height:1px;background:rgba(255,255,255,0.7);"></div>
  <div style="position:absolute;bottom:24px;right:24px;width:1px;height:70px;background:rgba(255,255,255,0.7);transform:translateX(69px);"></div>
  <div style="position:absolute;bottom:36px;right:36px;width:50px;height:1px;background:rgba(255,255,255,0.4);"></div>
  <div style="position:absolute;bottom:36px;right:36px;width:1px;height:50px;background:rgba(255,255,255,0.4);transform:translateX(49px);"></div>
</div>

<!-- タイトル下ゴールド横線 -->
<div style="position:absolute;top:50%;left:50%;transform:translate(-50%,20px);width:480px;height:1px;background:linear-gradient(90deg, #F8E6C8, #DDBE7B, #FFE9AC, #FDF3D5, #B19549);z-index:0;pointer-events:none;"></div>
```

---
【装飾 — コンテンツページ用】
上70%ライトグレー・下20%チャコール帯。

```html
<!-- 下部チャコール帯 -->
<div style="position:absolute;bottom:0;left:0;width:1280px;height:144px;background:#3A3A3A;z-index:1;pointer-events:none;"></div>

<!-- ゴールド区切り線 -->
<div style="position:absolute;bottom:144px;left:0;width:1280px;height:1px;background:linear-gradient(90deg, #F8E6C8, #DDBE7B, #FFE9AC, #FDF3D5, #B19549);z-index:2;pointer-events:none;"></div>
```

---
