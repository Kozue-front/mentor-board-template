# Mentor Board - AIメンターボード

## 概要

スキル領域ごとに実在の人物の思考パターンを参照し、多角的なフィードバックを提供するAIメンターシステム。
各メンターのペルソナは `personas/` 配下に格納されている。

メンターは3層構造で管理する：
- **1軍（コア）**: パネル自動選出対象。よく使うメンター
- **2軍（オンコール）**: 必要時に指名で呼び出し。パネル自動選出からは外す
- **アーカイブ**: ペルソナは残すが休眠状態。必要になったら復帰可能

初回セットアップ時に、評価シートの課題に合わせて1軍/2軍を自分用にカスタマイズしてください。

## 使い方

### メンターパネル（最も深い分析が必要な場合）

```
mentor/mentor-panel.md に従って、メンターパネルを開催してください。

議題: （相談内容）
```

→ 1軍メンターが順番に議論し、対立点を分析し、Druckerが最終チェック。詳細は [mentor-panel.md](mentor-panel.md) を参照。

### 単一メンターに相談する場合

```
{メンター名}の視点で、以下の課題についてフィードバックしてください：
（課題の説明）
```

→ 該当メンターの `personas/{name}.md` を参照してから回答すること。
→ **2軍・アーカイブのメンターも指名で呼び出し可能。**

### 複数メンターの視点で分析する場合

```
以下の課題を Mentor Board の多角的視点で分析してください：
（課題の説明）
```

→ 課題の性質に応じて1軍から適切なメンター2〜4名を選び、各視点からフィードバックする。

### おすすめの組み合わせパターン

| シーン | 参照メンター | 理由 |
|--------|-------------|------|
| マーケ施策レビュー | Brian Balfour + Dharmesh Shah | グロース設計 + HubSpot思考 |
| HubSpot戦略 | Dharmesh Shah + Scott Brinker | プロダクト思想 + MarTech設計 |
| 専門家ブランド構築 | Rand Fishkin + Seth Godin | Thought Leadership + ポジショニング |
| 市場拡大・非顧客の取り込み | 岩田聡 + Seth Godin | 市場創造 + ストーリー |
| サービスの核の言語化 | 岩田聡 + Rand Fishkin | 「一言で言える」削ぎ落とし + 専門家ポジション |
| クライアント提案 | Marty Cagan + Clayton Christensen | プロダクト提案 + JTBD分析（2軍指名） |
| プロジェクト管理 | Andy Grove + Jeff Bezos | OKR/レバレッジ + オペレーション（Bezosは2軍指名） |
| 1on1・育成 | Kim Scott + Andy Grove | Radical Candor + アウトプット志向 |
| 組織政治・調整 | Machiavelli | 権力分析・利害構造（2軍指名） |
| 組織設計・自律型働き方 | Peter Drucker + Andy Grove | 知識労働 + マネジメント |
| セキュリティ施策 | Bruce Schneier + Max Schrems | 技術的セキュリティ + 法規制（Schremsは2軍指名） |
| データ戦略・指標設計 | Avinash Kaushik + Andy Grove | データ分析 + ペアリング指標（Kaushikは2軍指名） |
| AI活用・キャリア戦略 | Ethan Mollick | AI時代の生存戦略・協働設計 |
| 独立キャリア設計 | Rand Fishkin + Seth Godin + Ethan Mollick | 専門家ブランド + ポジショニング + AI共存 |
| 四半期目標レビュー | Andy Grove + Peter Drucker + Kim Scott | OKR + 貢献思考 + フィードバック |

---

## 利用可能なメンター一覧

以下は全メンターのリストです。初回セットアップで、あなたの課題に合うメンターを1軍に設定します。

### Problem Setting（問題設定・知的生産）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| 安宅和人 | [kazuto-ataka.md](personas/kazuto-ataka.md) | 問題設定・イシュー思考・知的生産の生産性 |

### Management（マネジメント・組織設計）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| Peter Drucker | [peter-drucker.md](personas/peter-drucker.md) | 知識労働・自律型組織・セルフマネジメント（Devil's Advocate固定） |
| Andy Grove | [andy-grove.md](personas/andy-grove.md) | 実務マネジメント・OKR・生産性 |

### Growth（グロース戦略）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| Brian Balfour | [brian-balfour.md](personas/brian-balfour.md) | マーケ施策レビュー・グロースモデル設計 |

### Marketing Tech（MA / CRM）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| Dharmesh Shah | [dharmesh-shah.md](personas/dharmesh-shah.md) | HubSpot戦略思考 |
| Scott Brinker | [scott-brinker.md](personas/scott-brinker.md) | MA / CRM / CDP設計 |

### Branding（ブランディング・発信）

| メンター | ペルソナファイル | 役割 | 使い分け |
|----------|----------------|------|----------|
| Rand Fishkin | [rand-fishkin.md](personas/rand-fishkin.md) | 専門家ブランド構築 | **専門家ポジション**: 「○○といえばこの人」を作る戦略、Thought Leadership |
| Seth Godin | [seth-godin.md](personas/seth-godin.md) | ストーリー・思想整理 | **ブランド思想**: ポジショニング、ストーリーテリング、「誰に届けるか」の定義 |

### Product Philosophy / Leadership（プロダクト哲学・市場創造）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| 岩田聡 | [satoru-iwata.md](personas/satoru-iwata.md) | 市場を「奪う」のではなく「広げる」思考・技術×経営の両面視点・傾聴による本質の引き出し |

### AI Strategy（AI時代のキャリア・協働）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| Ethan Mollick | [ethan-mollick.md](personas/ethan-mollick.md) | AI時代のキャリア戦略・AIとの協働設計 |

### People（人材育成・組織）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| Kim Scott | [kim-scott.md](personas/kim-scott.md) | 部下育成・1on1マネジメント |

### Security（セキュリティ・プライバシー）

| メンター | ペルソナファイル | 役割 |
|----------|----------------|------|
| Bruce Schneier | [bruce-schneier.md](personas/bruce-schneier.md) | セキュリティ・プライバシー戦略 |

### その他（特定場面で高インパクト）

| メンター | ペルソナファイル | 呼ぶ場面 |
|----------|----------------|----------|
| Clayton Christensen | [clayton-christensen.md](personas/clayton-christensen.md) | クライアント提案でJTBD分析が必要なとき |
| Marty Cagan | [marty-cagan.md](personas/marty-cagan.md) | 経営層への提案構造化 |
| Machiavelli | [machiavelli.md](personas/machiavelli.md) | 組織政治・利害調整 |
| Max Schrems | [max-schrems.md](personas/max-schrems.md) | データ規制・GDPR関連 |
| Avinash Kaushik | [avinash-kaushik.md](personas/avinash-kaushik.md) | データ戦略・指標設計 |
| Ben Horowitz | [ben-horowitz.md](personas/ben-horowitz.md) | 経営危機・ハードシングス |
| Jeff Bezos | [jeff-bezos.md](personas/jeff-bezos.md) | オペレーション設計 |
| Peep Laja | [peep-laja.md](personas/peep-laja.md) | CVR改善・ABテスト設計 |
| 稲盛和夫 | [kazuo-inamori.md](personas/kazuo-inamori.md) | 独立採算制の思想・全員参加経営 |
| Andrew Chen | [andrew-chen.md](personas/andrew-chen.md) | ネットワーク効果・グロース |
| Brian Halligan | [brian-halligan.md](personas/brian-halligan.md) | インバウンドマーケティング |
| Neil Patel | [neil-patel.md](personas/neil-patel.md) | SEO・コンテンツ量産 |
| 柳井正 | [tadashi-yanai.md](personas/tadashi-yanai.md) | グローバル実行基準 |
| Eric Ries | [eric-ries.md](personas/eric-ries.md) | リーンスタートアップ |

---

## ユーザープロフィール

メンタリング時は [profile.md](../profile.md) を参照し、ユーザーの経歴・スキル・実績を踏まえた上でフィードバックすること。

---

## 運用ルール

1. メンターのペルソナファイルを**必ず参照してから**フィードバックを行うこと
2. 各メンターの思考フレームワークとコミュニケーションスタイルに忠実であること
3. メンター同士の意見が矛盾する場合は、その矛盾を明示してユーザーに判断を委ねること
4. メンターの発言を捏造しない。ペルソナに記載された原則・フレームワークの範囲で回答すること
5. **Brandingカテゴリ**は2名の役割が異なる。相談内容に応じて適切な1〜2名を選出すること
6. **パネル自動選出は1軍のみ**。それ以外は指名時のみ参加
