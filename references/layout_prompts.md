# レイアウト別プロンプトテンプレート v2

> 各レイアウト種別に対応するプロンプトテンプレート。
> `{{変数}}` は商品設計書の記載内容で置換する。
> 全プロンプトの末尾に `design_system.md` の共通デザイン指示を付加すること。
>
> **Canvaリファレンス画像**: 各レイアウトに対応するCanvaテンプレート画像を `references` に含めること。
> 画像パスは `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/` 以下。

---

## 目次

1. [cover（表紙）](#cover表紙) — `A_cover_title.jpg`
3. [bullet-list（箇条書き）](#bullet-list箇条書き) — `B_bullet_list.jpg`
4. [profile（講師プロフィール）](#profile講師プロフィール) — `C_profile.jpg`
5. [section-title（セクション扉）](#section-titleセクション扉) — `J_section_divider.jpg`
6. [two-column（2カラム）](#two-column2カラム) — `K_two_column_compare.jpg`
7. [phase-card（フェーズ説明）](#phase-cardフェーズ説明) — `H_curriculum_overview.jpg`
8. [feature-card（提供コンテンツ）](#feature-card提供コンテンツ) — `I_content_detail.jpg`
9. [comparison（比較表）](#comparison比較表) — `F_plan_comparison.jpg`
10. [pain-point（悩み・共感）](#pain-point悩み共感) — `B_bullet_list.jpg`
11. [pricing（価格提示）](#pricing価格提示) — `D_pricing_detail.jpg`
12. [market-price（業界相場）](#market-price業界相場) — `E_market_price.jpg`
13. [bonus（特典紹介）](#bonus特典紹介) — `L_bonus_feature.jpg`
14. [social-proof（実績）](#social-proof実績) — `M_social_proof.jpg`
15. [vip-bonus（VIP特典）](#vip-bonusVIP特典) — `N_vip_bonus.jpg`
16. [contrast（対比）](#contrast対比) — `G_impact_statement.jpg`
17. [cta（エンディング）](#ctaエンディング) — `O_closing_cta.jpg`
18. [payment（支払い方法）](#payment支払い方法) — `B_bullet_list.jpg`

---

## Canvaリファレンス画像パス一覧

| レイアウト | ファイル名 | フルパス |
|---|---|---|
| A 表紙 | A_cover_title.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/A_cover_title.jpg` |
| B 箇条書き | B_bullet_list.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/B_bullet_list.jpg` |
| C 自己紹介 | C_profile.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/C_profile.jpg` |
| D 商品金額 | D_pricing_detail.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/D_pricing_detail.jpg` |
| E 業界相場 | E_market_price.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/E_market_price.jpg` |
| F 商品一覧 | F_plan_comparison.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/F_plan_comparison.jpg` |
| H カリキュラム | H_curriculum_overview.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/H_curriculum_overview.jpg` |
| I 提供コンテンツ | I_content_detail.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/I_content_detail.jpg` |
| J セクション扉 | J_section_divider.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/J_section_divider.jpg` |
| K 2カラム比較 | K_two_column_compare.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/K_two_column_compare.jpg` |
| L 特典 | L_bonus_feature.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/L_bonus_feature.jpg` |
| M 社会的証明 | M_social_proof.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/M_social_proof.jpg` |
| N VIP特典 | N_vip_bonus.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/N_vip_bonus.jpg` |
| O クロージング | O_closing_cta.jpg | `/home/ubuntu/skills/product-slide-generator/templates/canva_reference/O_closing_cta.jpg` |

---

## cover（表紙）

**Canvaリファレンス**: `A_cover_title.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation cover slide.

LAYOUT:
- Center of slide: large title text "{{講座名}}" in elegant serif font, champagne gold color
- Below title: thin champagne gold horizontal divider line
- Below divider: subtitle "{{コンセプト（1行要約）}}" in clean sans-serif, dark charcoal gray
- Generous whitespace around all text elements
- Double thin gold frame border around the entire slide
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Title: "{{講座名}}"
- Subtitle: "{{コンセプト（1行要約）}}"
```

---

## bullet-list（箇条書き）

**Canvaリファレンス**: `B_bullet_list.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide with a header banner and bullet point list.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "{{見出し}}" in white, clean sans-serif font — NO logo
- Below banner: bullet points listed vertically with generous spacing between items
- Each bullet point prefixed with a right-pointing arrow "→" in champagne gold
- Wide letter-spacing, relaxed line-height (2.0x)
- Left-aligned text with generous left margin (15% from edge)
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "{{見出し}}"
- Arrow 1: "→ {{項目①}}"
- Arrow 2: "→ {{項目②}}"
- Arrow 3: "→ {{項目③}}"
[追加項目があれば続ける]
```

---

## profile（講師プロフィール）

**Canvaリファレンス**: `C_profile.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide for instructor profile.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "講師プロフィール" in white, clean sans-serif font — NO logo
- Left side (35% width): instructor photo area [写真指示をここに挿入]
- Right side (55% width): instructor information
  - Top: title/position "{{肩書き}}" in small text
  - Below: name "{{講師名}}" in large serif font, champagne gold
  - Below name: achievement list with bullet points, dark charcoal text
- Achievements listed with "・" prefix, generous line spacing
- Photo framed with thin champagne gold border
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "講師プロフィール"
- Title: "{{肩書き}}"
- Name: "{{講師名}}"
- Achievements:
  - "{{実績①}}"
  - "{{実績②}}"
  [続く]
```

---

## section-title（セクション扉）

**Canvaリファレンス**: `J_section_divider.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide serving as a section divider.

LAYOUT:
- NO header banner on this page
- Center of slide: large section title "{{セクション名}}" in elegant serif font, champagne gold
- Below title: thin champagne gold horizontal divider line
- Below divider: course name "{{講座名}}" in smaller sans-serif, dark charcoal gray
- Generous whitespace — text occupies only 40% of slide area
- Slightly more prominent corner decorations than content pages
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Section title: "{{セクション名}}"
- Course name: "{{講座名}}"
```

---

## two-column（2カラム）

**Canvaリファレンス**: `K_two_column_compare.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide with two-column layout.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "{{見出し}}" in white, clean sans-serif font — NO logo
- Left column (45% width): items listed vertically
  - "{{左カラム項目①}}"
  - "{{左カラム項目②}}"
  - "{{左カラム項目③}}"
- Right column (45% width): items listed vertically
  - "{{右カラム項目①}}"
  - "{{右カラム項目②}}"
  - "{{右カラム項目③}}"
- Thin vertical champagne gold divider line between columns
- Each item with generous vertical spacing
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "{{見出し}}"
[各項目のテキストをここに列挙]
```

---

## phase-card（フェーズ説明）

**Canvaリファレンス**: `H_curriculum_overview.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide explaining a course phase/stage.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "講座カリキュラム" in white, clean sans-serif font — NO logo
- Phase number and title: "Phase {{番号}}: {{タイトル}}" in champagne gold serif font
- Below: explanation text "{{説明文}}" in dark charcoal sans-serif
- If photo area exists: right side (40% width) with [写真指示]
- Generous whitespace between all elements
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "講座カリキュラム"
- Phase label: "Phase {{番号}}"
- Phase title: "{{タイトル}}"
- Description: "{{説明文}}"
```

---

## feature-card（提供コンテンツ）

**Canvaリファレンス**: `I_content_detail.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide showcasing a provided content/service.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "提供コンテンツ" in white, clean sans-serif font — NO logo
- Content number label "{{番号}}" in small champagne gold text below banner
- Center: content title "{{タイトル}}" in large serif font, champagne gold
- Below title: description "{{説明文}}" in dark charcoal sans-serif, generous line spacing
- Right or bottom area: sample image placeholder [写真指示 or プレースホルダー]
- Clean, spacious layout with text occupying max 60% of slide
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "提供コンテンツ"
- Number: "{{番号}}"
- Title: "{{タイトル}}"
- Description: "{{説明文}}"
```

---

## comparison（比較表）

**Canvaリファレンス**: `F_plan_comparison.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide with a comparison layout.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "プラン一覧" in white, clean sans-serif font — NO logo
- Two columns side by side
- Left column header: "{{左ラベル}}" (e.g., "スタンダード")
- Right column header: "{{右ラベル}}" (e.g., "VIP")
- Comparison items listed in rows below each header
- Right column items highlighted with champagne gold accent
- Thin divider line between columns
- Clean table-like layout without heavy borders
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "プラン一覧"
[比較項目をここに列挙]
```

---

## pain-point（悩み・共感）

**Canvaリファレンス**: `B_bullet_list.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide expressing empathy with audience pain points.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "{{見出し}}" in white, clean sans-serif font — NO logo
- Large empathetic text listed vertically below banner
- Text in dark charcoal gray, slightly larger than body text
- Items listed with generous spacing
- Subtle, warm atmosphere — NOT aggressive or alarming
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "{{見出し}}"
- "{{共感文 or 悩みリスト}}"
```

---

## pricing（価格提示）

**Canvaリファレンス**: `D_pricing_detail.jpg`（`references`に必ず含めること）
**レイアウト構造**: `layout_templates.md` の `=== LAYOUT STRUCTURE: PRICING ===` を必ず参照すること

```
A premium 16:9 presentation slide presenting pricing information.

IMPORTANT: Follow the LAYOUT STRUCTURE exactly as specified below.
Follow the COLOR and ATMOSPHERE from the theme reference image.
CRITICAL: The background MUST use the SAME gradient as the cover page — NOT a flat/solid color. Always reference the cover page generated image for background consistency.
Follow the COLOR and ATMOSPHERE from the theme reference image.
Do NOT modify the layout structure based on theme colors or decorations.
Do NOT add box/card/rectangle backgrounds around any text group.

LAYOUT (FIXED TWO-COLUMN STRUCTURE — DO NOT DEVIATE):
- LEFT COLUMN (30-35% width of slide):
  - Product/course name "{{講座名}}" at y=30-35%, left-aligned, serif font
  - Below: gold gradient horizontal accent line spanning column width
  - Below line: plan name "{{プラン名}}" in theme accent color
  - Below: price "{{価格}}" in LARGE gold gradient text (48-56px equivalent)
  - Below: "(税込)" in smaller gold text
  - Left margin: 5-8% from slide edge

- VERTICAL DIVIDER LINE:
  - Position: x=35-38% of slide width
  - Thin hair-line, spans y=8% to y=92%
  - Color: theme-appropriate (gold, silver, or muted)

- RIGHT COLUMN (60-65% width of slide):
  - Section 1 — "対象：" label in theme accent color (italic), y=10-12%
    - Content text in charcoal gray on same line or below
    - Thin horizontal separator line below
  - Section 2 — "期間：" label in theme accent color (italic)
    - Content text in charcoal gray
    - Thin horizontal separator line below
  - Section 3 — "提供内容" label in theme accent color, slightly larger
    - Content items listed below, each on its own line, charcoal gray

- NO header banner on this page
- NO box/card/rectangle backgrounds
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Course name: "{{講座名}}"
- Plan: "{{プラン名}}"
- Price: "{{価格}}"
- Target: "対象： {{対象}}"
- Duration: "期間： {{期間}}"
- Content label: "提供内容"
- Content items:
  [提供内容リスト — 各項目を1行ずつ]
```

---

## market-price（業界相場）

**Canvaリファレンス**: `E_market_price.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide showing industry standard pricing comparison.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "業界の相場" in white, clean sans-serif font — NO logo
- Visual price comparison showing industry average vs this course price
- Industry prices listed with large numbers, muted charcoal color
- This course price highlighted in champagne gold, larger font
- Arrow or visual indicator showing the value difference
- Clean, trustworthy layout
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "業界の相場"
[価格比較の詳細テキスト]
```

---

## bonus（特典紹介）

**Canvaリファレンス**: `L_bonus_feature.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide introducing a bonus/benefit.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "特典" in white, clean sans-serif font — NO logo
- Bonus number: "特典 {{番号}}" in small champagne gold text below banner
- Bonus title: "{{特典タイトル}}" in large serif font, champagne gold
- Description: "{{説明文}}" in dark charcoal sans-serif below
- Optional: image area on one side [写真指示 or プレースホルダー]
- Generous whitespace, premium feel
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "特典"
- Label: "特典 {{番号}}"
- Title: "{{特典タイトル}}"
- Description: "{{説明文}}"
```

---

## social-proof（実績）

**Canvaリファレンス**: `M_social_proof.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide showcasing achievements and social proof.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "受講生の実績" in white, clean sans-serif font — NO logo
- Achievement items or testimonials displayed prominently
- If photos available: arranged in a clean grid or gallery layout
- Numbers and statistics highlighted in large champagne gold font
- Professional, trustworthy atmosphere
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "受講生の実績"
[実績テキストをここに列挙]
```

---

## vip-bonus（VIP特典）

**Canvaリファレンス**: `N_vip_bonus.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide introducing VIP-exclusive benefits.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "VIP特典" in white, clean sans-serif font — NO logo
- VIP label prominently displayed in champagne gold
- Benefit title: "{{特典タイトル}}" in large serif font, champagne gold
- Description: "{{説明文}}" in dark charcoal sans-serif
- Optional: image area [写真指示 or プレースホルダー]
- Exclusive, premium atmosphere
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "VIP特典"
- Title: "{{特典タイトル}}"
- Description: "{{説明文}}"
```

---

## contrast（対比）

**Canvaリファレンス**: `G_impact_statement.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide with before/after or left/right contrast.

LAYOUT:
- NO header banner on this page (impact-style layout)
- Two halves side by side
- Left side: "{{左ラベル}}" header + description, slightly muted tone
- Right side: "{{右ラベル}}" header + description, champagne gold accent
- Clear visual distinction between the two sides
- Arrow or transition indicator between them
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Left: "{{左ラベル}}" / "{{左説明}}"
- Right: "{{右ラベル}}" / "{{右説明}}"
```

---

## cta（エンディング）

**Canvaリファレンス**: `O_closing_cta.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation closing slide with call to action.

LAYOUT:
- NO header banner on this page
- Center: CTA message "{{行動喚起メッセージ}}" in large serif font, champagne gold
- Below: course name "{{講座名}}" in smaller text
- Slightly more decorative than content pages — elegant closing feel
- Corner ornaments slightly more prominent
- Warm, inviting, confident atmosphere
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- CTA: "{{行動喚起メッセージ}}"
- Course: "{{講座名}}"
```

---

## payment（支払い方法）

**Canvaリファレンス**: `B_bullet_list.jpg`（`references`に必ず含めること）

```
A premium 16:9 presentation slide showing payment options.

LAYOUT:
- Top-left: header banner (dark charcoal rectangle #333333, width ~35% of slide, height ~8%)
  - Banner text: "お支払い方法" in white, clean sans-serif font — NO logo
- Payment options listed clearly with generous spacing:
  - "{{銀行振込の条件}}"
  - "{{クレジット分割の条件}}"
- Clean, trustworthy layout with clear information hierarchy
- NO logo, NO brand mark anywhere

TEXT (render exactly):
- Banner: "お支払い方法"
- Options: [支払い方法の詳細]
```
