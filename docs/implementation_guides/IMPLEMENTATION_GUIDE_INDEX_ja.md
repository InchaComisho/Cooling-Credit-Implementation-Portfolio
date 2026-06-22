# クーリングクレジット 段階的実装ガイド INDEX

## Step-by-Step Implementation Guides for Cooling Credits

[← クーリングクレジット実装ポートフォリオへ戻る](../../README_ja.md)  
[関連構想・実装候補リンク集へ戻る](../RELATED_IMPLEMENTATION_LINKS_ja.md)

---

## 概要

このページは、クーリングクレジットの実装候補を、企業、自治体、研究機関、地域事業者、農業者、都市設計者、海洋技術者が段階的に検討できるように整理した実装ガイドの索引である。

クーリングクレジットは、単一の技術ではない。

都市冷却、土壌再生、森林再生、有機資源循環、移動体冷却、砂漠再生、海洋循環、文明OSなどを、**熱負荷低減** という共通評価軸で接続する制度である。

そのため、実装も一つの手順だけではなく、分野ごとに異なる段階、測定項目、リスク管理、MRV設計が必要になる。

---

## 基本方針

この実装ガイド群は、以下の原則に基づく。

1. **小規模実証から始める**  
   いきなり大規模導入せず、測定可能な小規模プロジェクトから開始する。

2. **実測データを重視する**  
   気温、地表温度、WBGT、湿度、水使用量、電力使用量、土壌水分、植生変化などを記録する。

3. **Cooling Credit Score Estimator と接続する**  
   実測値を `Cooling-Credit-Framework` の試算モデルへ入力し、予備的な冷却貢献を評価する。

4. **リスクと停止条件を明確にする**  
   特に水ストレス、湿度悪化、生態系影響、海洋介入については、停止条件と監視体制を必ず設定する。

5. **正式認証ではなく予備評価として扱う**  
   現段階のスコアや仮クレジット単位は、制度設計・比較・MRV設計のための参考値であり、公式な取引クレジットではない。

---

## 実装ガイド一覧

### 1. 都市冷却ガイド

- [都市冷却・段階的実装ガイド](URBAN_COOLING_STEP_BY_STEP_GUIDE_ja.md)

対象例:

- 超音波ミスト冷却
- センター噴霧型ミスト冷却ファン
- 保水舗装
- 雨水貯留
- 街路樹
- 屋上緑化
- 壁面緑化
- 室外機吸気側プレクーリング
- 都市排熱削減

都市冷却は、比較的小規模な実証から始めやすい領域である。自治体、商店街、学校、公園、工場、駅前、屋外作業エリアなどで導入検討が可能である。

---

### 2. 海洋調律・OTU実証設計ガイド

- [海洋調律・OTU 段階的実証設計ガイド](OCEAN_TUNING_STEP_BY_STEP_GUIDE_ja.md)

対象例:

- OBS / Ocean Breathing System
- 深海エアレーション
- OTU / Ocean Tuning Unit
- 海洋表層熱の観測
- 鉛直循環の評価
- 溶存酸素の監視
- プランクトン支援条件の検討
- 海洋熱波リスクの予備評価

海洋系は、都市冷却や土壌再生とは異なり、すぐに現地実装すべき領域ではない。事前調査、数値モデル、法的許認可、第三者レビュー、環境監視、停止条件を前提にした段階的実証設計が必要である。

---

## 今後追加予定のガイド

今後、以下の分野別ガイドを追加できる。

- 土壌再生・腐葉土化ガイド
- 森林再生・放置杉林循環資産化ガイド
- 砂漠再生・有機物循環ガイド
- 移動体冷却・UHVガイド
- 農地冷却・有機栽培ガイド
- 水循環都市ガイド
- 企業向けMRV導入ガイド
- 自治体向けクーリングクレジット実証事業ガイド

---

## Cooling Credit Score Estimator との接続

実装ガイドで取得したデータは、以下の試算モデルに入力できる。

- [Cooling Credit Score Estimator 日本語README](https://github.com/InchaComisho/Cooling-Credit-Framework/blob/main/simulations/cooling_credit_score_estimator/README_ja.md)
- [Cooling Credit Score Estimator Python Script](https://github.com/InchaComisho/Cooling-Credit-Framework/blob/main/simulations/cooling_credit_score_estimator/cooling_credit_score_estimator.py)
- [入力CSV例](https://github.com/InchaComisho/Cooling-Credit-Framework/blob/main/simulations/cooling_credit_score_estimator/example_inputs.csv)

この試算モデルは、以下を評価する。

- 熱負荷低減
- 気化熱冷却
- WBGT改善
- 水循環回復
- 土壌保水回復
- 植生回復
- 排熱削減
- 生態系冷却力回復
- 水ストレスペナルティ
- 湿度リスクペナルティ
- 生態系リスクペナルティ
- エネルギー使用ペナルティ

---

## 注意事項

この実装ガイド群は、正式な認証基準、法的手続き、施工基準、海洋実験許可、環境アセスメントを置き換えるものではない。

特に海洋、河川、森林、農地、公共空間での実装には、地域法令、所有者許可、行政手続き、環境影響評価、専門家レビューが必要になる場合がある。

本ガイドは、クーリングクレジットを社会実装するための **予備設計・実証計画・MRV整理のための公開フレームワーク** である。

---

## 戻る

- [クーリングクレジット実装ポートフォリオ](../../README_ja.md)
- [関連構想・実装候補リンク集](../RELATED_IMPLEMENTATION_LINKS_ja.md)
