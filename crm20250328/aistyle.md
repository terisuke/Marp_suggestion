---
marp: true
theme: default
paginate: true
style: |
  table {
    font-size: 0.75em;
  }
  .comparison {
    display: flex;
    justify-content: space-between;
    gap: 1rem;
    font-size: 0.8em;
  }
  .comparison-item {
    flex: 1;
  }
  .comparison-item ul {
    margin-top: 0.2em;
    margin-bottom: 0.2em;
    padding-left: 1.2em;
  }
  .comparison-item li {
    margin-bottom: 0.05em;
  }
  .comparison-item h3 {
    margin-top: 0.4em;
    margin-bottom: 0.2em;
  }
  blockquote {
    font-size: 0.8em;
    margin-top: 0.4em;
    margin-bottom: 0.4em;
  }
  blockquote p {
    margin: 0.2em 0;
  }
  .mvp-section {
    font-size: 0.8em;
  }
  .mvp-section h3 {
    margin-top: 0.4em;
    margin-bottom: 0.2em;
  }
  .mvp-section h2 {
    margin-top: 0.6em;
    margin-bottom: 0.2em;
  }
  .mvp-section ul, .mvp-section ol {
    margin-top: 0.2em;
    margin-bottom: 0.2em;
    padding-left: 1.2em;
  }
  .mvp-section li {
    margin-bottom: 0.05em;
  }
  .mvp-section p {
    margin: 0.2em 0;
  }
  .overview-section {
    font-size: 0.75em;
  }
  .overview-section h2 {
    margin-top: 0.5em;
    margin-bottom: 0.1em;
  }
  .overview-section ul {
    margin-top: 0.1em;
    margin-bottom: 0.1em;
    padding-left: 1.2em;
  }
  .overview-section li {
    margin-bottom: 0.02em;
  }
  h1 {
    margin-bottom: 0.5em;
  }
  h2 {
    margin-top: 0.5em;
    margin-bottom: 0.3em;
  }
  h3 {
    margin-top: 0.4em;
    margin-bottom: 0.2em;
  }
  ul, ol {
    margin-top: 0.2em;
    margin-bottom: 0.2em;
  }
  li {
    margin-bottom: 0.05em;
  }
  section {
    margin-top: 0.5em;
  }
  .compact {
    margin-top: 0.2em;
    margin-bottom: 0.2em;
  }

---

# AI活用型開発プロセス (建設業向け含む)
## 経営改善計画分析ツール開発計画
### **MVP + 建設業務管理モジュール**を一体化

---

# 目次

1. 開発概要とAI活用方針  
2. 全体機能一覧（経営改善 + 建設業務）  
3. AI活用による工数削減と費用シミュレーション  
4. 開発スケジュール（3ヶ月以内）  
5. 開発体制とリソース計画  
6. MVPリリース計画（Supabase + Next.js）  

---

# 1. 開発概要とAI活用方針

<div class="overview-section compact">

## 背景
<ul>
<li>既存の「経営改善計画.xlsx」を活用した財務分析やSWOT提案をWeb化</li>
<li><strong>建設業向け工事台帳、工程管理、写真・報告機能</strong>も含めた形で、一体のDXプラットフォームを構築</li>
<li><strong>Supabase プロジェクトは既に作成済み</strong></li>
<li><strong>フロントエンドのモック（Next.jsベース）も既に存在</strong></li>
</ul>

## 目的
<ul>
<li>財務データ分析から改善施策提案までをAIで効率化（中小企業向け）</li>
<li>建設業の現場管理DX（工程表、工事台帳、写真管理）と経営改善を一括サポート</li>
<li><strong>3ヶ月以内</strong>、<strong>125万円</strong>でPoC（MVP）を完成させる</li>
</ul>

## AI活用方針
<ul>
<li>Excel構造解析、財務分析、レポート自動生成でAIを活用</li>
<li>AIコーディング支援（Copilot, Cursorなど）で工数を30%以上削減</li>
<li>要件定義やドキュメント作成もChatGPT Proで加速</li>
</ul>

</div>

---

# 2. 全体機能一覧（経営改善 + 建設業務）

| カテゴリ              | 代表的な機能                                                   | AI活用ポイント                                                               |
|-------------------|----------------------------------------------------------|------------------------------------------------------------------------|
| 経営改善支援      | Excel取込・財務分析<br>SWOT分析<br>アクションプラン生成                | Excel構造解析と自動マッピング<br>財務指標計算・異常値検出<br>ChatGPTによる戦略提案 |
| 計数計画・シミュレーション | 売上・利益シミュレーション<br>KPI管理<br>レポート出力                      | 経営指標の自動計算と可視化<br>LLMを活用した改善案提案<br>レポート自動生成         |
| 建設業務管理      | 工程表（ガントチャート）<br>工事台帳（契約・請書管理）<br>写真・報告アップロード | ガントチャート自動生成（AI補助）<br>写真分析（将来的にAI物体認識）<br>報告書のPDF生成 |
| ダッシュボードと通知機能  | 進捗状況可視化<br>Slack/LINE通知<br>経営状況ハイライト             | リアルタイム分析（Supabase）<br>通知トリガーの自動設定<br>AIによる重要アラート要約           |

---

# 3. AI活用による工数削減と費用シミュレーション

| 項目                     | 従来工数 (4.4人月) | AI活用工数 (3人月) | 削減率    | 開発費用              |
|------------------------|------------------|------------------|-----------|---------------------|
| 経営改善機能 (Excel分析) | 2.1人月            | 1.3人月            | 38%       | 1.3 × 40万円 = 52万円 |
| 建設業務管理             | 2.3人月            | 1.7人月            | 26%       | 1.7 × 40万円 = 68万円 |
| **合計**                 | **4.4人月**        | **3.0人月**        | **約30%** | **125万円**           |

> **注:** AIコーディング支援、ドキュメント生成、テスト自動化により **約3.0人月に圧縮**  
> 人月単価は40万円で算出  
> ツール利用料（数万円）含めても125万円が目安

---

# 4. 開発スケジュール（3ヶ月以内）

## フェーズと期間比較

| フェーズ                         | 従来期間   | AI活用期間 | 短縮率    |
|------------------------------|-----------|-----------|-----------|
| Phase 0: 要件定義/設計       | 0.8ヶ月     | 0.4ヶ月     | 50%       |
| Phase 1: MVP実装 (経営+建設) | 2.0ヶ月     | 1.2ヶ月     | 40%       |
| Phase 2: テスト/統合/リリース準備   | 1.6ヶ月     | 1.0ヶ月     | 37%       |
| **合計**                     | **4.4ヶ月** | **2.6ヶ月** | **約40%** |

**ただしAI活用により更なる短縮が期待→ 3ヶ月内で完了可能**

---

# 5. 開発体制とリソース計画

<div class="comparison">
<div class="comparison-item">

### 従来型
<ul>
<li>PM: 1名</li>
<li>バックエンド: 1-2名</li>
<li>フロント: 1名</li>
<li>デザイナー: 0.5名</li>
<li>テスター: 0.5名</li>
<li><strong>計: 4-5名</strong></li>
</ul>

</div>
<div class="comparison-item">

### AI活用型
<ul>
<li>PM兼AI導入担当: 1名</li>
<li>フルスタックエンジニア (Next.js + Supabase): 1名</li>
<li>若手エンジニア (AI補助で学習しながら実装): 1名</li>
<li>財務・建設アドバイザー: 0.3名 (パート)</li>
<li><strong>計: 3-3.3名</strong></li>
</ul>

</div>
</div>

> **ポイント:**  
> 1. SupabaseプロジェクトおよびMockフロントが既に存在  
> 2. AIで実装/ドキュメント化/テストを効率化  
> 3. 3名程度で3ヶ月 → 125万円

---

# 6. MVPリリース計画 (Supabase + Next.js)

<div class="mvp-section">

### 前提
<ul>
<li><strong>既にSupabaseプロジェクトを作成</strong></li>
<li><strong>Next.jsベースのモックUI</strong>があり、そこへ機能統合</li>
</ul>

## MVPの範囲
<ol>
<li><strong>財務分析 (Excel取込)</strong> + <strong>アクションプラン生成</strong></li>
<li><strong>建設業務管理 (工事台帳 + 工程表 + 写真アップロード)</strong></li>
<li>ダッシュボードと通知 (Slack/LINEなど)</li>
</ol>

## 納期と費用
<ul>
<li><strong>約3ヶ月以内</strong>にPoC完成</li>
<li><strong>総額125万円</strong> (人件費 + AIツール利用料)</li>
</ul>

<p><strong>AI活用で短期開発 & コスト抑制。現場でのPoC検証後、必要に応じて拡張。</strong></p>

</div>

---

# まとめ: AI連携で「経営 + 建設」DXをスピード実現

- **経営改善DX** と **建設業務DX** を最初から一体化 → 重複作業を排除
- **既存モック + Supabase** を活用し、機能をAIで一気に実装
- 3名体制 × 3ヶ月、**125万円**でPoCリリース
- さらなる拡張（AI写真解析、工数集計、自動レポート）も段階的に対応可能
