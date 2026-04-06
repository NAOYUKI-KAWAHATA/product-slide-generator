# デザインシステム v2: モノトーン＋シャンパンゴールド（受講生配布版）

> このファイルは全ページの画像生成プロンプトに**共通で付加する**デザイン指示である。
> `layout_prompts.md` のレイアウト別プロンプトと組み合わせて使用する。

---

## 見出しバナーのルール（最重要）

### ルール1: 見出しバナーは全コンテンツページで完全統一

コンテンツページ（表紙・セクション扉・インパクト文ページ以外の全ページ）には、**必ず以下の統一デザインの見出しバナーを表示する**。

```
HEADER BANNER (MANDATORY for all content pages):
- Position: top-left corner of the slide
- Shape: horizontal rectangle banner, width ~35% of slide, height ~8% of slide
- Background: dark charcoal gray (#333333) — same on EVERY content page
- Text: section label "{{見出し}}" in white, clean sans-serif font, medium weight
- NO logo, NO icon, NO brand mark — text only
- The banner shape, color, and font MUST be IDENTICAL across all content pages
- NEVER change the banner design between slides
```

### ルール2: 見出しバナーが不要なページ

以下のページには見出しバナーを表示しない：
- 表紙（cover）
- セクション扉（section-title）
- インパクト文ページ（statement）— 大きな1文のみのページ

### ルール3: ロゴ・ブランドマークは一切表示しない

- 「M」ロゴ、MUGEN LABロゴ、その他いかなるブランドマークも表示しない
- ロゴエリアは空白のまま

---

## 共通デザイン指示（英文ブロック — 全ページのプロンプト末尾に付加）

```
=== DESIGN SYSTEM: MONOTONE + CHAMPAGNE GOLD v2 ===

BACKGROUND:
- Base: white to light gray gradient with subtle white marble texture
- Corners and edges: thin champagne gold geometric lines and subtle ornamental accents
- Center area: clean and uncluttered, ensuring maximum text readability
- Thin double gold frame border around the entire slide (like an elegant picture frame)
- NO heavy patterns, NO busy textures in the text area
- Overall brightness: bright and airy, NOT dark or heavy

COLOR PALETTE:
- Background: white (#FFFFFF) to light warm gray (#F5F3F0)
- Primary text: dark charcoal gray (#333333 to #444444)
- Title text: champagne gold (#B8976A) with subtle gradient to (#C5A55A)
- Accent lines: champagne gold (#C5A55A), thin and refined
- Decorative elements: muted gold, never overpowering

TYPOGRAPHY RULES:
- Titles: elegant serif font, champagne gold color, generous letter-spacing (tracking: wide)
- Body text: clean sans-serif font, dark charcoal gray, comfortable letter-spacing
- Line height: relaxed and spacious (1.8x to 2.0x for body text)
- Character spacing: wide and breathable, NEVER cramped
- Font size hierarchy: maintain clear visual hierarchy between title, subtitle, and body

TEXT COLOR RULES (CRITICAL):
- COVER and SECTION TITLE pages ONLY: main title may use gold or gradient color
- ALL OTHER PAGES: body text, bullet points, descriptions MUST be charcoal gray (#333333) or white (#FFFFFF)
- NEVER use gradient text on body copy, bullet points, or descriptions
- NEVER use gold text on body copy — gold is reserved for titles on cover/section pages only
- Banners, decorative elements, divider lines: gold and gradients are acceptable
- The goal is READABILITY and SOPHISTICATION, not visual spectacle

SPACING AND WHITESPACE:
- Generous margins on all sides (minimum 8% of slide width)
- Ample breathing room between text blocks
- Text should occupy no more than 65% of the slide area
- "Less is more" — prioritize readability over information density

HEADER BANNER RULE (CRITICAL — NEVER VIOLATE):
- ALL content pages MUST have a header banner in the top-left corner
- Banner: dark charcoal rectangle (#333333), width ~35% of slide, height ~8%
- Banner text: white, clean sans-serif, section label only — NO logo, NO brand mark
- The banner design MUST be IDENTICAL on every content page — same shape, same color, same font
- Pages WITHOUT banner: cover page, section-title pages, statement (single large text) pages
- DO NOT add any logo or brand mark anywhere on any slide

DECORATIVE ELEMENTS:
- Champagne gold horizontal divider line below section titles (thin, 1-2px)
- Corner ornaments: subtle geometric gold lines at 2-4 corners only
- All decorations are SUPPORTING ROLE ONLY, never competing with text

MOOD AND ATMOSPHERE:
- Sophisticated adult luxury with understated elegance
- Like a premium hotel lobby or high-end magazine editorial
- Calm confidence, NOT flashy or aggressive
- Matte finish feel, NOT glossy or shiny

=== STRICT RULES — DO NOT VIOLATE ===
- DO NOT make the overall slide dark or heavy — keep it bright and airy
- DO NOT use flashy or glittery gold effects — use matte champagne gold only
- DO NOT crowd text — always maintain generous whitespace
- DO NOT let decorative elements obscure or compete with text
- DO NOT use more than 3 font sizes per slide
- DO NOT add any logo, brand mark, or "M" symbol anywhere
- ENSURE all Japanese text is rendered EXACTLY as written — no missing, garbled, or incorrect characters
- ENSURE text-to-background contrast ratio is at least 4.5:1
- ENSURE consistent visual style across all slides in the presentation
- ENSURE the header banner design is IDENTICAL on every content page
- ENSURE the overall impression is: sophisticated, premium, understated luxury

=== ANTI-GLITTER RULES — STRICTLY ENFORCED ===
- DO NOT use gradient text on body copy or bullet points — this looks cheap and AI-generated
- DO NOT use rainbow, neon, or overly saturated colors anywhere
- DO NOT use heavy gloss, chrome, or mirror effects
- DO NOT use excessive sparkle, lens flare, or light burst effects
- DO NOT use more than ONE decorative technique per slide (e.g., if using gold ribbon, skip sparkles)
- KEEP decorative elements subtle and supporting — they should be barely noticeable at first glance
- The test: if someone looks at the slide and says "wow that's flashy", it has failed
- The goal: someone looks at the slide and says "this looks expensive and professional"
```

---

## カラーコード早見表

| 用途 | カラー | HEX |
|---|---|---|
| 背景（白） | ピュアホワイト | #FFFFFF |
| 背景（グレー） | ウォームライトグレー | #F5F3F0 |
| 本文テキスト | ダークチャコール | #333333 |
| サブテキスト | ミディアムグレー | #666666 |
| タイトル | シャンパンゴールド | #B8976A |
| アクセント | ゴールド | #C5A55A |
| フレーム | ライトゴールド | #D4C5A0 |
| 見出しバナー背景 | ダークチャコール | #333333 |
| 見出しバナーテキスト | ホワイト | #FFFFFF |

---

## 写真プレースホルダーの指示

写真が未提供の場合、以下のプロンプトを使用する。

### プロフィール写真（おまかせ生成時）

```
In the photo area, render a professional business portrait:
- Japanese [male/female], [age]s
- Wearing a sophisticated dark business attire
- Confident, warm, approachable expression
- Studio lighting with soft key light
- 4K photorealistic quality, NOT AI-looking
- Natural skin texture, realistic proportions
- Framed in an elegant champagne gold picture frame
```

### イベント・セミナー写真（おまかせ生成時）

```
In the photo area, render a professional seminar/event scene:
- Japanese audience in a modern, well-lit conference room
- Professional atmosphere, engaged participants
- Warm lighting, clean environment
- 4K photorealistic quality
```

### 写真枠（ユーザー提供待ち）

```
In the photo area, render a light gray placeholder rectangle (#E0E0E0)
with a thin champagne gold border and a small camera icon in the center.
Label: "写真" in small gray text below the placeholder.
```
