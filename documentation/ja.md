<!-- ELUCENIA technical documentation · wells-tep · ja · no clinical/professional/rights approval -->

# Wellsスコア（肺塞栓症）

[条件・出典・許諾](https://elucenia.org/ja/tools/wells-tep)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 深部静脈血栓症の臨床徴候

`tvp`

### 肺塞栓症が最も可能性の高い診断

`alt`

### 心拍数 \> 100 bpm

`fc`

### ≥ 3日の不動または過去4週間以内の手術

`imob`

### 深部静脈血栓症または肺塞栓症の既往

`prev`

### 喀血

`hemo`

### 活動性がん（過去6か月以内の治療、または緩和治療）

`cancer`

## 方法の版

Wells PE 2000：7加重因子；2段階と3段階分類を区別

## 記載された計算式

合計点：DVT徴候3 · PEの方が可能性が高い3 · 心拍数\>100は1.5 · 不動/手術1.5 · DVT/PE既往1.5 · 喀血1 · がん1。

## 限界・対象集団

肺塞栓症のWellsスコアは、臨床的に疑われる人を対象に、スコアとDダイマーを組み合わせる方針の中で研究されました。二段階と三段階の分類では閾値が異なり、低スコアや塞栓症の可能性が低いことは、塞栓症がないことと同義ではありません。Dダイマー測定法と適用基準は、使用する診断プロトコルに対応する必要があります。

## 参考文献

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
