<!-- ELUCENIA technical documentation · calcio-corrigido · ja · no clinical/professional/rights approval -->

# アルブミン補正カルシウム

[条件・出典・許諾](https://elucenia.org/ja/tools/calcio-corrigido)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 総カルシウム

`ca`

mg/dL · 範囲: 2–20

### アルブミン

`alb`

g/dL · 範囲: 0.5–6

## 方法の版

Payne 1973に関連する簡易補正：Ca+0.8×(4−アルブミン)；イオン化カルシウムの実測ではありません

## 記載された計算式

補正カルシウム (mg/dL) = 総カルシウム + 0.8 × (4.0 − アルブミン（g/dL）).

mmol/Lの場合：カルシウム + 0.02 × (40 − アルブミン（g/L）).

## 限界・対象集団

Payne 1973の論文の式は、肝機能検査に提出された蛋白異常のある検体から導出され、アルブミンの係数は1、カルシウムの単位はmg/100 mL、アルブミンの単位はg/100 mLです。ローカルの簡略変法は0.8を使用しており、この変更自体の出典が必要です。補正カルシウムは推定値で、イオン化カルシウムの測定ではありません。

## 参考文献

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

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
