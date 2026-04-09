# レイアウト構造テンプレート（Layout Structure Templates）

> **目的**: 各ページタイプの「構造・配置・余白」を厳密に定義する。
> テーマが変わっても、このレイアウト構造は**絶対に変わらない**。
>
> **使い方**: `image_slide_generate` のプロンプト作成時に、該当するレイアウトテンプレートの
> STRUCTURE セクションを**そのままコピー**してプロンプトに含めること。
> テーマの色・装飾は `design_themes.md` から上書きする。
>
> **最重要ルール**: レイアウト構造はCanvaリファレンス画像＋このファイルの定義に従う。
> テーマの色や装飾がレイアウト構造を変更することは**絶対にない**。

---

## レイアウトタイプ一覧

| ID | タイプ名 | Canvaリファレンス | テーマリファレンス | 用途 |
|---|---|---|---|---|
| A | cover | A_cover_title.jpg | cover.png | 表紙 |
| B | bullet-list | B_bullet_list.jpg | bullet_list.png | 箇条書き・コンセプト・悩み共感 |
| C | profile | C_profile.jpg | content.png | 講師プロフィール |
| D | pricing | D_pricing_detail.jpg | pricing.png | 料金・プラン詳細 |
| E | market-price | E_market_price.jpg | pricing.png | 業界相場比較 |
| F | comparison | F_plan_comparison.jpg | pricing.png | プラン一覧比較 |
| H | phase-card | H_curriculum_overview.jpg | content.png | カリキュラム・フェーズ説明 |
| I | feature-card | I_content_detail.jpg | content.png | 提供コンテンツ詳細 |
| J | section-title | J_section_divider.jpg | cover.png | セクション扉 |
| K | two-column | K_two_column_compare.jpg | content.png | 2カラム比較 |
| L | bonus | L_bonus_feature.jpg | content.png | 特典紹介 |
| M | social-proof | M_social_proof.jpg | content.png | 実績・社会的証明 |
| N | vip-bonus | N_vip_bonus.jpg | content.png | VIP特典 |
| O | cta | O_closing_cta.jpg | cover.png | エンディング・CTA |

---

## A: cover（表紙）

**Canvaリファレンス**: `A_cover_title.jpg`
**テーマリファレンス**: `cover.png`

```
=== LAYOUT STRUCTURE: COVER ===

POSITION & SIZING:
- Title: centered horizontally, positioned at vertical 40-45% of slide
- Title font size: very large (equivalent to 72-80px)
- Thin horizontal line: directly below title, width ~40% of slide, centered
- Subtitle: centered horizontally, positioned 5-8% below the line
- Subtitle font size: medium (equivalent to 24-28px)

SPACING:
- Top margin: 35-40% of slide height (generous empty space above title)
- Bottom margin: 30-35% of slide height
- Gap between title and line: 2%
- Gap between line and subtitle: 3-5%

ELEMENTS:
- NO header banner
- NO logo, NO brand mark
- Decorative elements: theme-defined (corners only, never center)

ALIGNMENT: All elements centered horizontally
===
```

---

## B: bullet-list（箇条書き・コンセプト）

**Canvaリファレンス**: `B_bullet_list.jpg`
**テーマリファレンス**: `bullet_list.png`

```
=== LAYOUT STRUCTURE: BULLET-LIST ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35% of slide, height ~7-8%
  - Text: white, centered within banner
- Content area: below banner, LEFT-ALIGNED
  - Left margin: 8-10% from left edge
  - Top of first item: 22-25% from top

SPACING:
- Between bullet items: generous vertical gap (minimum 8-10% of slide height)
- 3 items should be distributed across vertical 25%-75% of slide
- Each line breathes with ample whitespace above and below
- Line height within each item: relaxed (1.8-2.0x)

ELEMENTS:
- Header banner (theme-colored gradient + white text)
- 3-5 text items, left-aligned
- NO bullet markers unless theme specifies (theme may use → or ◆)
- Decorative elements: theme-defined (corners only)

ALIGNMENT: Text LEFT-ALIGNED (NOT centered)
===
```

---

## D: pricing（料金・プラン詳細）

**Canvaリファレンス**: `D_pricing_detail.jpg`
**テーマリファレンス**: `pricing.png`

```
=== LAYOUT STRUCTURE: PRICING ===

CRITICAL: This layout has a FIXED two-column structure. Do NOT deviate.

POSITION & SIZING:
- LEFT COLUMN (30-35% width):
  - Product/course name: positioned at y=30-35%, left-aligned within column
  - Gold horizontal accent line: below product name, spanning column width
  - Plan name: below gold line, theme accent color
  - Price: below plan name, LARGE (equivalent to 48-56px), gold gradient
  - Price label "(税込)": smaller, same gold tone
  - All left column text: left-aligned with 5-8% left margin

- VERTICAL DIVIDER LINE:
  - Position: x=35-38% of slide width
  - Spans from y=8% to y=92%
  - Hair-thin line, theme-appropriate color

- RIGHT COLUMN (60-65% width):
  - Section 1 "対象：": starts at y=10-12%
    - Label "対象：" in theme accent color (italic if theme supports)
    - Content text in charcoal gray, same line or below
    - Horizontal separator line below (thin, theme-colored)
  - Section 2 "期間：": starts below separator
    - Label "期間：" in theme accent color
    - Content text in charcoal gray
    - Horizontal separator line below
  - Section 3 "提供内容": starts below separator
    - Label "提供内容" in theme accent color, slightly larger
    - Content list below in charcoal gray, each item on its own line

SPACING:
- Right column sections: evenly distributed with generous gaps
- Horizontal separator lines: thin, extend ~90% of right column width
- Between content items in "提供内容": comfortable line spacing (1.6-1.8x)

ELEMENTS:
- NO header banner on this page
- NO box/card/rectangle backgrounds around any text group
- Vertical divider line between columns
- Horizontal separator lines between right-side sections
- Decorative elements: theme-defined (corners only)

ALIGNMENT: Left column left-aligned, right column left-aligned
===
```

---

## E: market-price（業界相場）

**Canvaリファレンス**: `E_market_price.jpg`
**テーマリファレンス**: `pricing.png`

```
=== LAYOUT STRUCTURE: MARKET-PRICE ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Price comparison items: listed vertically below banner
  - Left margin: 10%
  - Each item: category label + price
- Industry prices: muted charcoal color
- This course price: highlighted in gold, larger font
- Visual indicator (arrow or line) showing value difference

SPACING:
- Between price items: 6-8% vertical gap
- Generous whitespace around highlighted price

ALIGNMENT: Left-aligned
===
```

---

## F: comparison（プラン一覧比較）

**Canvaリファレンス**: `F_plan_comparison.jpg`
**テーマリファレンス**: `pricing.png`

```
=== LAYOUT STRUCTURE: COMPARISON ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Two columns below banner, equal width
  - Left column header: plan name (e.g., "スタンダード")
  - Right column header: plan name (e.g., "VIP"), gold accent
- Comparison items in rows below headers
- Thin vertical divider between columns

SPACING:
- Between comparison rows: 4-6% vertical gap
- Column headers: prominent, 15% from top

ALIGNMENT: Each column internally left-aligned
===
```

---

## H: phase-card（カリキュラム・フェーズ説明）

**Canvaリファレンス**: `H_curriculum_overview.jpg`
**テーマリファレンス**: `content.png`

```
=== LAYOUT STRUCTURE: PHASE-CARD ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Phase number + title: below banner, left-aligned
  - Position: y=18-22%, x=8%
  - Phase number in accent color, title in charcoal
- Description text: below phase title
  - Position: y=35-40%, x=8%
  - Width: max 55% of slide
- Optional image area: right side (35-40% width)

SPACING:
- Between phase number and description: 8-10%
- Generous whitespace around all elements

ALIGNMENT: Left-aligned
===
```

---

## I: feature-card（提供コンテンツ詳細）

**Canvaリファレンス**: `I_content_detail.jpg`
**テーマリファレンス**: `content.png`

```
=== LAYOUT STRUCTURE: FEATURE-CARD ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Content number: small accent text below banner, x=8%, y=15%
- Content title: large text, x=8%, y=22-28%
- Description: below title, x=8%, width max 55%
- Optional image area: right side or bottom

SPACING:
- Between title and description: 5-8%
- Generous line spacing in description (1.6-1.8x)

ALIGNMENT: Left-aligned
===
```

---

## C: profile（講師プロフィール）

**Canvaリファレンス**: `C_profile.jpg`
**テーマリファレンス**: `content.png`

```
=== LAYOUT STRUCTURE: PROFILE ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Left side (30-35% width): instructor photo area
  - Photo: centered within left column, y=25-70%
  - Thin border around photo (theme-colored)
- Right side (55-60% width):
  - Title/position: small text, y=20%
  - Name: large serif font, gold accent, y=28-32%
  - Achievement list: below name, bullet points with "・" prefix

SPACING:
- Between name and achievements: 5%
- Between achievement items: 3-4%

ALIGNMENT: Left side centered, right side left-aligned
===
```

---

## J: section-title（セクション扉）

**Canvaリファレンス**: `J_section_divider.jpg`
**テーマリファレンス**: `cover.png`

```
=== LAYOUT STRUCTURE: SECTION-TITLE ===

POSITION & SIZING:
- Section title: centered, y=40-45%, large serif font
- Thin horizontal line: below title, centered, width ~30%
- Course name: below line, centered, smaller font

SPACING:
- Text occupies only 40% of slide area
- Generous margins on all sides

ELEMENTS:
- NO header banner
- Slightly more prominent corner decorations than content pages

ALIGNMENT: All centered
===
```

---

## K: two-column（2カラム比較）

**Canvaリファレンス**: `K_two_column_compare.jpg`
**テーマリファレンス**: `content.png`

```
=== LAYOUT STRUCTURE: TWO-COLUMN ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Left column: x=5-8%, width=40%
- Right column: x=52-55%, width=40%
- Thin vertical divider: centered between columns

SPACING:
- Items within each column: 5-7% vertical gap
- Top of content: y=18-22%

ALIGNMENT: Each column left-aligned
===
```

---

## L: bonus（特典紹介）

**Canvaリファレンス**: `L_bonus_feature.jpg`
**テーマリファレンス**: `content.png`

```
=== LAYOUT STRUCTURE: BONUS ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Bonus number: small accent text, x=8%, y=15%
- Bonus title: large text, x=8%, y=22-28%
- Description: below title, x=8%, width max 55%
- Optional image: right side

SPACING:
- Between title and description: 5-8%
- Generous whitespace

ALIGNMENT: Left-aligned
===
```

---

## M: social-proof（実績・社会的証明）

**Canvaリファレンス**: `M_social_proof.jpg`
**テーマリファレンス**: `content.png`

```
=== LAYOUT STRUCTURE: SOCIAL-PROOF ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- Achievement items or testimonials: below banner
- Numbers/statistics: large font, gold accent
- Photos (if available): grid or gallery layout

SPACING:
- Between items: generous vertical gap
- Statistics prominently sized

ALIGNMENT: Varies by content (centered for stats, left for testimonials)
===
```

---

## N: vip-bonus（VIP特典）

**Canvaリファレンス**: `N_vip_bonus.jpg`
**テーマリファレンス**: `content.png`

```
=== LAYOUT STRUCTURE: VIP-BONUS ===

POSITION & SIZING:
- Header banner: top-left corner, compact rectangle
  - Position: x=3%, y=3%
  - Size: width ~30-35%, height ~7-8%
- VIP label: prominent, gold accent, y=15-18%
- Benefit title: large text, x=8%, y=25-30%
- Description: below title, x=8%, width max 55%

SPACING:
- Generous whitespace, exclusive premium feel
- Between title and description: 5-8%

ALIGNMENT: Left-aligned
===
```

---

## O: cta（エンディング・CTA）

**Canvaリファレンス**: `O_closing_cta.jpg`
**テーマリファレンス**: `cover.png`

```
=== LAYOUT STRUCTURE: CTA ===

POSITION & SIZING:
- Main CTA message: centered, y=35-40%, large font
- Subtitle/instruction: centered, below main message
- Contact info or URL: centered, y=65-70%

SPACING:
- Generous margins, clean and open
- Text occupies max 60% of slide width

ELEMENTS:
- NO header banner
- Decorative elements: theme-defined (corners, slightly more prominent)

ALIGNMENT: All centered
===
```

---

## レイアウト適用ルール（必読）

1. **プロンプト作成時**: 該当レイアウトの `=== LAYOUT STRUCTURE ===` ブロックを**そのまま**プロンプトに含める
2. **references配列**: 必ず以下の順で画像を含める
   - [0] Canvaリファレンス画像（レイアウト構造の参照）
   - [1] テーマリファレンス画像（色・装飾の参照）
   - [2] 直前ページの生成画像（デザイン継続性）
3. **プロンプト内に必ず以下を明記**:
   ```
   IMPORTANT: Follow the LAYOUT STRUCTURE exactly as specified.
   Follow the COLOR and ATMOSPHERE from the theme reference image.
   Do NOT modify the layout structure based on theme colors or decorations.
   ```
4. **レイアウトの変更は禁止**: テーマが変わっても、要素の配置・サイズ・余白は同一
5. **色・装飾のみテーマで変更**: バナーの色、テキストの色、装飾要素のみテーマに従う
