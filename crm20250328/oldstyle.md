---
marp: true
theme: default
paginate: true
style: |
  table {
    font-size: 0.8em;
  }
  .comparison {
    display: flex;
    justify-content: space-between;
    gap: 1rem;
  }
  .comparison-item {
    flex: 1;
  }

---

# 従来型開発プロセス
## 経営改善計画分析ツール開発計画
### 包括的経営改善支援システム

---

# 目次

1. 開発概要
2. 経営改善計画Excelの分析
3. 機能一覧と工数
4. 開発スケジュール
5. 費用とリソース計画
6. MVPリリース計画

---

# 1. 開発概要

## 目的
- 既存の「経営改善計画.xlsx」を活用した経営改善支援システム
- 企業の財務データを分析し経営改善策を提案するソフト
- 中小企業の経営改善プロセスを支援するクラウドプラットフォーム

## 特徴
- Excel形式の経営改善計画をシステム化
- 財務分析から戦略立案、実行計画までを統合
- 使いやすいインターフェースで経営改善を効率化

---

# 2. 経営改善計画Excelの分析

## 経営改善計画Excel - 主要シート構成

| カテゴリ     | 主なシート                                                | 目的                                                        |
|----------|------------------------------------------------------|-----------------------------------------------------------|
| メタ情報   | メニュー、概要                                             | 全体のナビゲーション、計画の目的や背景説明                             |
| 現状分析 | 過去BS・PL・CF、過去コスト情報、得意先・店舗別等、資産保全状況 | 財務状況の把握、コスト構造の分析、収益構造の分析、担保・資産状況の確認 |
| 戦略立案 | ビジネスモデル俯瞰図、SWOT分析                                | 事業構造の可視化、強み弱み機会脅威の分析                         |
| 実行計画 | アクションプラン、計数計画、月間収支計画、年間資金繰り計画        | 具体的な実行計画、数値目標の設定、月次の収支予測、資金繰りの見通し   |

---

## Excel活用の意義と課題

<div class="comparison">
<div class="comparison-item">

### 意義
- ユーザーが馴染みのある形式
- 既存データの活用が容易
- 柔軟な拡張性

</div>
<div class="comparison-item">

### 課題
- 複雑なシート構造の理解
- シート間の関連性の把握
- データの整合性確保
- ユーザーインターフェースの改善

</div>
</div>

---

# 3. 機能一覧と工数

| 機能               | 概要               | 開発工数 | 費用    |
|--------------------|------------------|--------|-------|
| Excel構造解析・取込 | 既存エクセルの読込と解析 | 1.0人月  | 80万円  |
| 現状分析機能       | 財務・コスト・顧客分析  | 1.2人月  | 96万円  |
| 戦略立案支援       | SWOT分析・戦略提案  | 1.3人月  | 104万円 |
| 実行計画・シミュレーション  | アクションプラン・計数予測  | 0.8人月  | 64万円  |
| レポート・ダッシュボード       | 分析・提案の可視化   | 0.7人月  | 56万円  |

※人月単価は80万円で計算
**合計: 5.0人月 (400万円)**

---

# 主要機能の詳細

## Excel構造解析・取込機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 経営改善計画Excelの取込と解析
- シート間の関連性・数式の理解
- データ項目の自動マッピング

</div>
<div class="comparison-item">

### 技術要件
- 複雑なExcel構造の解析
- データの整合性チェック
- エラー検出と修正提案

</div>
</div>

**工数**: 1.0人月
**担当者**: バックエンドエンジニア 1名

---

## 現状分析機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 財務データ・コスト分析
- 顧客分析
- 業界比較

</div>
<div class="comparison-item">

### 技術要件
- 財務比率の計算と評価
- トレンド分析とグラフ化
- 業界平均との比較

</div>
</div>

**工数**: 1.2人月
**担当者**: バックエンド 1名、財務アナリスト 0.5名

---

## 戦略立案支援機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- SWOT分析
- ビジネスモデル可視化
- 戦略提案

</div>
<div class="comparison-item">

### 技術要件
- SWOT要素の整理と分析
- 戦略オプションの提示
- ビジネスモデルの可視化

</div>
</div>

**工数**: 1.3人月
**担当者**: バックエンド 1名、ビジネスアナリスト 0.5名

---

## 実行計画・シミュレーション機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- アクションプラン立案
- 計数計画
- 資金繰り予測

</div>
<div class="comparison-item">

### 技術要件
- 施策の優先順位付け
- 数値計画の作成支援
- シナリオに基づく予測

</div>
</div>

**工数**: 0.8人月
**担当者**: バックエンドエンジニア 1名

---

## レポート・ダッシュボード機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 分析レポート生成
- 進捗管理
- KPI可視化

</div>
<div class="comparison-item">

### 技術要件
- PDF/Excel形式レポート出力
- インタラクティブダッシュボード
- KPI進捗モニタリング

</div>
</div>

**工数**: 0.7人月
**担当者**: フロントエンド 1名

---

# 4. 開発スケジュール

## 開発フェーズと期間

| フェーズ                        | 内容                   | 期間       |
|-----------------------------|------------------------|-----------|
| Phase 0: 要件定義とExcel分析 | Excel構造詳細分析と設計 | 0.6ヶ月     |
| Phase 1: コア機能開発         | 基本機能実装           | 1.8ヶ月     |
| Phase 2: 機能統合とテスト       | 機能統合とQA            | 1.2ヶ月     |
| Phase 3: MVPリリース準備        | 最終調整とリリース          | 0.6ヶ月     |
| Phase 4: 機能拡張と改善      | 追加機能開発           | 3-4ヶ月〜    |
| **合計開発期間**            |                        | **4.2ヶ月** |

---

## Phase 0: 要件定義とExcel分析 (0.6ヶ月)

<div class="comparison">
<div class="comparison-item">

### 作業内容
- 経営改善計画Excelの詳細分析
- システム要件の定義
- データモデルの設計
- 開発計画の詳細化

</div>
<div class="comparison-item">

### 成果物
- Excel構造分析書
- 要件定義書
- データモデル設計書
- 開発計画書

</div>
</div>

---

## Phase 1: コア機能開発 (1.8ヶ月目)

<div class="comparison">
<div class="comparison-item">

### 作業内容
- Excel解析・取込機能実装
- 現状分析・戦略立案機能実装
- ユーザーインターフェース開発
- 基本機能の実装

</div>
<div class="comparison-item">

### 成果物
- 基本システム
- 共通コンポーネント
- 基本機能の実装

</div>
</div>

---

## Phase 2: 機能統合とテスト (1.2ヶ月目)

<div class="comparison">
<div class="comparison-item">

### 作業内容
- 実行計画・シミュレーション機能実装
- レポート・ダッシュボード実装
- 総合テスト実施
- 不具合修正

</div>
<div class="comparison-item">

### 成果物
- 全機能の実装
- 統合テスト結果
- 修正報告書

</div>
</div>

---

## Phase 3: MVPリリース準備 (0.6ヶ月目)

<div class="comparison">
<div class="comparison-item">

### 作業内容
- 最終調整
- ドキュメント作成
- デプロイ準備
- ユーザー受入テスト

</div>
<div class="comparison-item">

### 成果物
- テスト結果報告書
- ユーザーマニュアル
- 管理者ガイド
- APIドキュメント

</div>
</div>

**MVPリリース**

---

# 5. 費用とリソース計画

## 従来型開発の総費用

<div class="comparison">
<div class="comparison-item">

### 開発工数
- 総工数: 約5.0人月
- 人月単価: 80万円
- 総開発費用: 約400万円

</div>
<div class="comparison-item">

### 人員構成
- プロジェクトマネージャー: 1名
- バックエンドエンジニア: 1-2名
- フロントエンドエンジニア: 1名
- 財務/ビジネスアナリスト: 1名
- テスター: 0.5名 (兼任)
- **合計: 4.5-5.5名体制**

</div>
</div>

---

# 6. MVPリリース計画

## MVP(最小実用製品)の範囲

<div class="comparison">
<div class="comparison-item">

### 基本機能
- Excel取込・分析基盤
- 現状診断機能
- 改善計画支援
- 基本レポート

</div>
<div class="comparison-item">

### 開発計画
- 開発工数: 約4.0人月
- 開発人数: 4-5名体制
- 開発期間: 約4.2ヶ月

</div>
</div>

**「確実な品質確保」と「基本機能の完全実装」を重視**

---

# まとめ: 従来型開発アプローチ

<div class="comparison">
<div class="comparison-item">

### 開発規模
- 開発期間: 4.2ヶ月
- 総開発費用: 400万円
- 開発工数: 5.0人月
- 開発体制: 4.5-5.5名

</div>
<div class="comparison-item">

### 特徴
- 堅実な計画
- 確実な品質担保
- 段階的な開発
- 経験者中心の体制

</div>
</div>

**堅実な計画で確実に品質を担保**