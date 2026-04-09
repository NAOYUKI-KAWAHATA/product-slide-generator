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

TYPOGRAPHY (CRITICAL — OVERRIDES DEFAULT):
- ALL text on ALL pages MUST use a feminine Japanese serif (Mincho) typeface — elegant, thin strokes
- NEVER use Gothic (sans-serif) typeface anywhere — not for titles, not for body, not for banners
- Heading banner text: white Mincho serif
- Body text: charcoal gray Mincho serif
- Title text: dusty gradient Mincho serif

BACKGROUND:
- Cover page: white (#FFFFFF) with very subtle gradient to pale pink (#FFF0F5) and pale lavender (#F0E6FF)
- Content pages: ALMOST PURE WHITE (#FFFFFF to #FFFBFD) — gradient must be barely perceptible, much lighter than cover page
- Content page gradient should be at most 5% opacity — the page should read as "white with a whisper of color"
- Soft, diffused light glow in bottom-right corner
- Overall: delicate, feminine, refined elegance

COLOR PALETTE:
- Background: white → pale pink (#FFF0F5) → pale lavender (#F0E6FF)
- Primary text: charcoal gray (#4A4A4A)
- Title text (cover/section ONLY): DUSTY muted blue-to-purple-to-pink gradient (#7A9BBF → #9B7FB8 → #C48A9F). NOT vivid or saturated — muted, dusty, sophisticated.
- Accent: subtle gold (#C5A55A) for price highlights only
- Heading banner: soft dusty pink-to-lavender gradient (#D4A0B0 → #B0A0C8) with white text
- Bullet icons: diamond (◆) shape in dusty pink-purple

DECORATIVE ELEMENTS:
- VERY THIN silver (#C0C0C0 / #D0D0D0) diamond-shaped line outlines — hair-thin strokes, barely visible
- Placed ONLY in top-left corner and bottom-right corner as a SYMMETRICAL PAIR
- Top-left: 2-3 small diamond outlines in thin silver lines, fading inward
- Bottom-right: 2-3 small diamond outlines in thin silver lines, fading inward (mirror of top-left)
- Diamond lines must NOT be assertive — they should be so subtle you almost miss them
- NO diamonds in the center or other areas — keep the center clean and open
- NO thick lines, NO bold strokes, NO filled diamonds — outlines only, hair-thin silver
- Controlled light particles — barely visible, like dust in sunlight
- NO heavy glow, NO lens flare, NO sparkle clusters
- Delicate and feminine — like fine lace or silk texture

TEXT SPACING (CRITICAL FOR CONTENT PAGES):
- Generous line spacing between bullet points — each line should breathe with ample whitespace above and below
- 3-line bullet lists should be evenly distributed across the vertical center of the slide with wide gaps between lines
- Text should feel spacious and airy, never cramped or dense
- Minimum 60px visual gap between each bullet line

MOOD: Delicate feminine elegance — like a luxury bridal magazine. Refined, soft, never loud. Every element whispers rather than shouts.
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

MOOD: Like a premium coastal spa brochure — cool, calming, refreshing. The mint-green background has a COOL BLUE undertone like sea glass or eucalyptus. NEVER warm, NEVER yellow-toned, NEVER matcha-like. Think: cool ocean breeze through mint leaves.

CRITICAL REMINDERS FOR ALL PAGES:
1. Background MUST be the same soft gradient on EVERY page (cover, content, pricing, ending). NEVER use a flat/solid color.
2. Background is primarily WHITE with a whisper of cool mint. NOT a green slide — a WHITE slide with green accents.
3. The bottom wave decoration MUST be cool blue-green (#8FA89A), NOT matcha/olive.
4. Keywords: 爽やかさ・清潔感・安らぎ (freshness, cleanliness, serenity).
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
