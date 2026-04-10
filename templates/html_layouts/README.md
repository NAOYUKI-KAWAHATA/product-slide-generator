# HTMLレイアウトテンプレート ガイド

## 概要

全13種類のHTMLレイアウトテンプレート。Canvaリファレンス画像の文字サイズ・余白・構造を忠実に再現している。テーマの色・装飾はテーマ変数（`{{THEME_VAR}}`）で差し替える。

## テンプレート一覧

| # | ファイル名 | レイアウト名 | 用途 | 対応Canvaリファレンス |
|---|----------|-----------|------|-----------------|
| 1 | `01_cover.html` | cover（表紙） | P1 | A_cover_title |
| 2 | `02_bullet_arrow.html` | bullet-arrow（矢印付き箇条書き） | P2 コンセプト | B_bullet_list |
| 3 | `03_bullet_list.html` | bullet-list（箇条書きリスト） | P22-P53 お悩み・特徴等 | B_bullet_list |
| 4 | `04_profile.html` | profile（講師プロフィール） | P4 | C_profile |
| 5 | `05_section_title.html` | section-title（セクション扉） | P5,P9,P21等 | H/J_section_divider |
| 6 | `06_two_column_chapter.html` | two-column-chapter（章立て2カラム） | P6 | K_two_column_compare |
| 7 | `07_phase_card.html` | phase-card（フェーズカード） | P7,P8 | 独自 |
| 8 | `08_feature_card.html` | feature-card（提供コンテンツ簡易） | P11-P19 | E_market_price |
| 9 | `09_feature_card_detail.html` | feature-card-detail（提供コンテンツ詳細） | P10 | I_content_detail |
| 10 | `10_content_summary.html` | content-summary（まとめ） | P20 | 独自 |
| 11 | `11_impact_statement.html` | impact-statement（インパクト文） | P3 | G_impact_statement |
| 12 | `12_pricing.html` | pricing（料金詳細） | P56-P61 | D_pricing_detail |
| 13 | `13_closing.html` | closing（エンディングCTA） | P62-P66 | O_closing_cta |

## 文字サイズ基準（Canvaリファレンス準拠）

| 要素 | サイズ | ウェイト |
|------|-------|---------|
| 表紙タイトル | 72px | 700 |
| セクション扉タイトル | 72px | 700 |
| バナー見出し | 36px | 700 |
| 本文（箇条書き3行） | 38px | 800 |
| 本文（箇条書き5-7行） | 26-32px | 700 |
| インパクト文 | 34px | 700 |
| コンテンツタイトル | 48px | 800 |
| 説明文 | 28px | 500 |
| サブタイトル | 24px | 400 |
| プロフィール名前 | 48px | 800 |
| プロフィール実績 | 22px | 500 |
| エンディングメッセージ | 44px | 700 |

## テーマ変数

各テンプレートの `{{VARIABLE}}` を、選択されたテーマの色に置き換えて使用する。共通変数は以下の通り。

| 変数名 | 説明 |
|--------|------|
| `{{BG_COLOR}}` | コンテンツページ背景色 |
| `{{BG_GRADIENT}}` | 表紙/プロフィール背景グラデーション |
| `{{BG_GRADIENT_DARK}}` | セクション扉/インパクト文の暗い背景 |
| `{{BANNER_BG}}` | 見出しバナー背景 |
| `{{TEXT_COLOR}}` | 本文テキスト色 |
| `{{TITLE_COLOR}}` | タイトル色 |
| `{{RULE_COLOR}}` | 水平線・区切り線の色 |
| `{{DECO_LEFT}}` | 左端の装飾要素（テーマ固有HTML） |
| `{{DECO_RIGHT_BOTTOM}}` | 右下の装飾要素（テーマ固有HTML） |
