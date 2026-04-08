# デザインシステム v3: テーマ対応版（受講生配布版）

> このファイルは全ページの画像生成プロンプトに**共通で付加する**デザイン指示である。
> `layout_prompts.md` のレイアウト別プロンプトと組み合わせて使用する。
>
> **テーマ別の色・装飾は `design_themes.md` で定義する。**
> このファイルはテーマに依存しない「構造・ルール」のみを定義する。

---

## 見出しバナーのルール（最重要）

### ルール1: 見出しバナーは全コンテンツページで完全統一

コンテンツページ（表紙・セクション扉・インパクト文ページ以外の全ページ）には、**必ず統一デザインの見出しバナーを表示する**。

```
HEADER BANNER (MANDATORY for all content pages):
- Position: top-left corner of the slide
- Shape: horizontal rectangle banner, width ~35% of slide, height ~8% of slide
- Background: use the theme's heading banner color (defined in design_themes.md)
- Text: section label "{{見出し}}" in white, clean sans-serif font, medium weight
- NO logo, NO icon, NO brand mark — text only
- The banner shape, position, and font MUST be IDENTICAL across all content pages
- ONLY the banner color changes per theme — the structure is always the same
- NEVER change the banner design between slides within the same presentation
```

### ルール2: 見出しバナーが不要なページ

以下のページには見出しバナーを表示しない：
- 表紙（cover）
- セクション扉（section-title）
- インパクト文ページ（statement）— 大きな1文のみのページ

### ルール3: ロゴ・ブランドマークは一切表示しない

- いかなるロゴ、ブランドマーク、シンボルも表示しない
- ロゴエリアは空白のまま

---

## 共通デザイン指示（英文ブロック — 全ページのプロンプト末尾に付加）

> **注意**: 以下の `COLOR PALETTE` と `DECORATIVE ELEMENTS` セクションはデフォルト値。
> テーマが選択された場合、`design_themes.md` の `=== THEME OVERRIDE ===` ブロックの
> 該当セクションで上書きすること。

```
=== DESIGN SYSTEM: COMMON RULES v3 ===

TYPOGRAPHY RULES:
- Titles: elegant font, generous letter-spacing (tracking: wide)
- Body text: clean sans-serif font, comfortable letter-spacing
- Line height: relaxed and spacious (1.8x to 2.0x for body text)
- Character spacing: wide and breathable, NEVER cramped
- Font size hierarchy: maintain clear visual hierarchy between title, subtitle, and body

TEXT COLOR RULES (CRITICAL — OVERRIDES ALL THEME SETTINGS):
- COVER and SECTION TITLE pages ONLY: main title may use theme accent color or gradient
- ALL OTHER PAGES: body text, bullet points, descriptions MUST be charcoal gray (#333333) or white (#FFFFFF)
- NEVER use gradient text on body copy, bullet points, or descriptions
- Banners, decorative elements, divider lines: theme colors and gradients are acceptable
- The goal is READABILITY and SOPHISTICATION, not visual spectacle

SPACING AND WHITESPACE:
- Generous margins on all sides (minimum 8% of slide width)
- Ample breathing room between text blocks
- Text should occupy no more than 65% of the slide area
- "Less is more" — prioritize readability over information density

HEADER BANNER RULE (CRITICAL — NEVER VIOLATE):
- ALL content pages MUST have a header banner in the top-left corner
- Banner: theme-colored rectangle, width ~35% of slide, height ~8%
- Banner text: white, clean sans-serif, section label only — NO logo, NO brand mark
- The banner design MUST be IDENTICAL on every content page — same shape, same position, same font
- Pages WITHOUT banner: cover page, section-title pages, statement (single large text) pages
- DO NOT add any logo or brand mark anywhere on any slide

=== STRICT RULES — DO NOT VIOLATE ===
- DO NOT crowd text — always maintain generous whitespace
- DO NOT let decorative elements obscure or compete with text
- DO NOT use more than 3 font sizes per slide
- DO NOT add any logo, brand mark, or symbol anywhere
- ENSURE all Japanese text is rendered EXACTLY as written — no missing, garbled, or incorrect characters
- ENSURE text-to-background contrast ratio is at least 4.5:1
- ENSURE consistent visual style across all slides in the presentation
- ENSURE the header banner design is IDENTICAL on every content page

=== ANTI-GLITTER RULES — STRICTLY ENFORCED ===
- DO NOT use gradient text on body copy or bullet points — this looks cheap and AI-generated
- DO NOT use rainbow, neon, or overly saturated colors anywhere
- DO NOT use heavy gloss, chrome, or mirror effects
- DO NOT use excessive sparkle, lens flare, or light burst effects
- DO NOT use more than ONE decorative technique per slide
- KEEP decorative elements subtle and supporting — they should be barely noticeable at first glance
- The test: if someone looks at the slide and says "wow that's flashy", it has FAILED
- The goal: someone looks at the slide and says "this looks expensive and professional"
```

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
with a thin border in theme accent color and a small camera icon in the center.
Label: "写真" in small gray text below the placeholder.
```
