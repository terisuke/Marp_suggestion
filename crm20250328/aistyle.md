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

# AI活用型開発プロセス
## Web会計ソフト開発計画
### freee類似サービス構築

---

# 目次

1. 開発概要とAI活用方針
2. 機能一覧と工数削減効果
3. AI活用型開発スケジュール
4. 費用とリソース計画
5. MVPリリース計画

---

# 1. 開発概要とAI活用方針

## 目的
- 中小企業のExcel経理業務をクラウド会計ソフトで効率化
- AIツールをフル活用し、開発効率を飛躍的に向上

## AI活用の基本方針
- コード生成AIによる実装の高速化
- UI/UXのAI自動デザイン
- テスト自動生成によるQA効率化
- プロジェクト管理の最適化

---

# AI活用によるメリット

<div class="comparison">
<div class="comparison-item">

## 従来型
- 開発期間: 4.0ヶ月
- 開発コスト: 400-480万円
- 開発体制: 4-5名
- 品質管理: 手動レビュー

</div>
<div class="comparison-item">

## AI活用型
- 開発期間: 2.8ヶ月
- 開発コスト: 148万円
- 開発体制: 3-4名
- 品質管理: AI自動レビュー

</div>
</div>

---

# 2. 機能一覧と工数削減効果

| 機能                | 従来工数    | AI活用工数 | 削減率 | AI活用費用 |
|-------------------|-----------|----------|--------|----------|
| 経費精算            | 1.0人月     | 0.5人月    | 50%    | 20万円     |
| 仕訳自動化          | 1.0人月     | 0.6人月    | 40%    | 24万円     |
| 帳簿作成・レポート       | 1.5人月     | 0.8人月    | 47%    | 32万円     |
| 請求書発行・売上管理 | 1.0人月     | 0.5人月    | 50%    | 20万円     |
| 決済・支払管理       | 0.5-1.0人月 | 0.3人月    | 40-70% | 12万円     |

※人月単価は経験の浅いエンジニアを想定して40万円で計算

---

# 主要機能の詳細とAI活用ポイント

## 機能構成
1. 経費精算システム
2. 仕訳自動化システム
3. 帳簿作成・レポートシステム
4. 請求書発行・売上管理システム
5. 決済・支払管理システム

---

## 経費精算機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 従業員の経費申請
- 承認ワークフロー
- 振込データ作成

</div>
<div class="comparison-item">

### AI活用ポイント
- フォーム自動生成
- バリデーションコード自動実装
- OCR精度向上

</div>
</div>

**工数**: 0.5人月 (50%削減)
**費用**: 20万円

---

## 仕訳自動化機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 銀行API連携
- 明細自動取得
- 仕訳ルール設定

</div>
<div class="comparison-item">

### AI活用ポイント
- API連携コード自動生成
- パターン学習による仕訳推論
- LLMによる明細分類

</div>
</div>

**工数**: 0.6人月 (40%削減)
**費用**: 24万円

---

## 帳簿作成・レポート機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 総勘定元帳生成
- 試算表出力
- 月次・年次決算書

</div>
<div class="comparison-item">

### AI活用ポイント
- レポートテンプレート自動生成
- 集計ロジック自動実装
- テストケース自動生成

</div>
</div>

**工数**: 0.8人月 (47%削減)
**費用**: 32万円

---

## 請求書発行・売上管理機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 請求書PDF出力
- インボイス対応
- 入金管理ダッシュボード

</div>
<div class="comparison-item">

### AI活用ポイント
- 請求書テンプレート自動生成
- PDF生成コード自動実装
- 入金予測モデル組込み

</div>
</div>

**工数**: 0.5人月 (50%削減)
**費用**: 20万円

---

## 決済・支払管理機能

<div class="comparison">
<div class="comparison-item">

### 基本機能
- 振込データ出力
- 支払スケジュール管理
- 一括振込処理

</div>
<div class="comparison-item">

### AI活用ポイント
- 銀行フォーマット対応の自動化
- 支払スケジュール最適化AI
- セキュリティチェック自動化

</div>
</div>

**工数**: 0.3人月 (40-70%削減)
**費用**: 12万円

---

# 使用するAIツール・技術

<div class="comparison">
<div class="comparison-item">

## 開発支援
- GitHub Copilot
- Claude Code
- AI UI/UXデザインツール

</div>
<div class="comparison-item">

## 品質管理
- AI自動テスト生成
- LLMによる仕様理解
- AIセキュリティスキャナー

</div>
</div>

---

# 3. AI活用型開発スケジュール

## 開発フェーズと期間比較

| フェーズ                       | 従来期間 | AI活用期間 | 短縮率 |
|----------------------------|---------|-----------|--------|
| Phase 0: 要件定義と基本設計 | 0.5ヶ月   | 0.3ヶ月     | 40%    |
| Phase 1: コア機能開発        | 2.0ヶ月   | 1.2ヶ月     | 40%    |
| Phase 2: 残り機能開発と統合  | 3.0ヶ月   | 1.8ヶ月     | 40%    |
| Phase 3: MVPリリース準備       | 4.0ヶ月   | 2.3ヶ月     | 43%    |
| Phase 4: 機能拡張と改善     | 5-6ヶ月〜  | 2.3-3ヶ月〜  | 50%+   |

---

## Phase 0: 要件定義と基本設計 (0.3ヶ月)

<div class="comparison">
<div class="comparison-item">

### 従来型
- 手動での要件収集
- 手動でのデータモデル設計
- 手動での画面設計
- 手動での要件解釈

</div>
<div class="comparison-item">

### AI活用型
- AIによるインタビュー分析
- AI支援ツールでの設計
- AIデザインツールでのプロトタイピング
- LLMによる要件解釈支援

</div>
</div>

**従来比: 40%時間短縮**

---

## Phase 1: コア機能開発 (1.2ヶ月目)

<div class="comparison">
<div class="comparison-item">

### 従来型
- 手動コーディング
- 手動でのCI/CD構築
- 手動でのコンポーネント開発
- 手動でのフレームワーク選定

</div>
<div class="comparison-item">

### AI活用型
- GitHub Copilotによるコード生成
- CI/CD構築の自動化
- 共通コンポーネントのAI生成
- AIによるフレームワーク選定支援

</div>
</div>

**従来比: 40%時間短縮**

---

## Phase 2: 残り機能開発と統合 (1.8ヶ月目)

<div class="comparison">
<div class="comparison-item">

### 従来型
- 手動での機能統合テスト
- 手動でのコードレビュー
- 手動でのデータ移行
- 手動でのAPI実装

</div>
<div class="comparison-item">

### AI活用型
- AI自動テスト生成
- AIツールによるコードレビュー
- AI生成のデータ移行ツール
- AIコード生成によるAPI実装

</div>
</div>

**従来比: 40%時間短縮**

---

## Phase 3: MVPリリース準備 (2.3ヶ月目)

<div class="comparison">
<div class="comparison-item">

### 従来型
- 手動でのセキュリティレビュー
- 手動でのドキュメント作成
- 手動でのパフォーマンス最適化
- 手動でのユーザー受入テスト

</div>
<div class="comparison-item">

### AI活用型
- AIツールによるセキュリティレビュー
- AIによるドキュメント生成
- AI分析ツールによる最適化
- AI支援のユーザー受入テスト

</div>
</div>

**従来比: 43%時間短縮**

---

## Phase 4: 機能拡張と改善 (2.3-3ヶ月目以降)

<div class="comparison">
<div class="comparison-item">

### 従来型
- 手動でのフィードバック分析
- 手動でのプライオリティ付け
- 手動での拡張機能開発

</div>
<div class="comparison-item">

### AI活用型
- AIによるフィードバック分析
- AI分析によるプライオリティ最適化
- AIコード生成による拡張機能開発

</div>
</div>

**従来比: 50%以上の時間短縮**

---

# 4. 費用とリソース計画

## AI活用型開発の総費用

<div class="comparison">
<div class="comparison-item">

### 従来型
- 開発工数: 5-6人月
- 人月単価: 80万円
- 総開発費用: 400-480万円

</div>
<div class="comparison-item">

### AI活用型
- 開発工数: 2.7人月
- 人月単価: 40万円
- 総開発費用: 108万円

</div>
</div>

※金融業向け追加対応含む場合: 3.7人月、148万円

---

## AI活用型の人員構成

<div class="comparison">
<div class="comparison-item">

### 従来型
- プロジェクトマネージャー: 1名
- バックエンドエンジニア: 1-2名
- フロントエンドエンジニア: 1名
- デザイナー: 0.5名
- テスター: 0.5名
- **合計: 4-5名**

</div>
<div class="comparison-item">

### AI活用型
- プロジェクトマネージャー: 1名
- フルスタックエンジニア: 1-2名
- 若手エンジニア: 1名
- **合計: 3-4名**

</div>
</div>

**特徴: 少人数でも高い生産性**
**人月単価: 40万円** (経験の浅いエンジニアでもAI活用で高生産性)

---

# 5. MVPリリース計画

## MVP(最小実用製品)の範囲

<div class="comparison">
<div class="comparison-item">

### 従来型
- 開発工数: 5-6人月
- 開発人数: 2-3名
- 開発期間: 4ヶ月

</div>
<div class="comparison-item">

### AI活用型
- 開発工数: 2.7人月
- 開発人数: 2-3名
- 開発期間: 2.3ヶ月

</div>
</div>

**「早期リリース」+「コスト削減」+「品質確保」の三方良し**

---

# 金融業向け追加対応とコスト

<div class="comparison">
<div class="comparison-item">

### 従来型
- セキュリティ強化: 別途
- コンプライアンス対応: 別途
- 追加コスト: 別途
- 期間延長: 別途

</div>
<div class="comparison-item">

### AI活用型
- セキュリティ強化: +0.5人月 (20万円)
- コンプライアンス対応: +0.5人月 (20万円)
- 追加コスト: 40万円
- 期間延長: +0.5ヶ月 (2.8ヶ月)

</div>
</div>

---

# AI活用における注意点

<div class="comparison">
<div class="comparison-item">

### 技術面
- 生成コードのレビュー必須
- 法規制対応の検証
- 知的財産権の確認
- セキュリティ配慮

</div>
<div class="comparison-item">

### 運用面
- AIツールの選定
- チームのAIスキル育成
- プロセスの最適化
- 品質管理の徹底

</div>
</div>

---

# AI人材育成のメリット

<div class="comparison">
<div class="comparison-item">

### 個人
- AIツール活用スキル
- プロンプトエンジニアリング
- 最新技術への対応力
- 生産性向上

</div>
<div class="comparison-item">

### 組織
- 少人数での高品質開発
- コスト削減
- 開発期間短縮
- 競争力向上

</div>
</div>

---

# まとめ: AI活用型開発アプローチ

<div class="comparison">
<div class="comparison-item">

### 従来型
- 開発期間: 4ヶ月
- 総開発費用: 400-480万円
- 開発工数: 5-6人月
- 人月単価: 80万円
- 開発体制: 4-5名

</div>
<div class="comparison-item">

### AI活用型
- 開発期間: 2.8ヶ月
- 総開発費用: 148万円
- 開発工数: 3.7人月
- 人月単価: 40万円
- 開発体制: 3-4名

</div>
</div>

**AI活用で「速く・安く・良く」を実現**