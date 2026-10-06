<!-- ELUCENIA technical documentation · calcio-corrigido · zh · no clinical/professional/rights approval -->

# 白蛋白校正钙

[条件、来源与许可](https://elucenia.org/zh/tools/calcio-corrigido)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 总钙

`ca`

mg/dL · 范围: 2–20

### 白蛋白

`alb`

g/dL · 范围: 0.5–6

## 方法版本

与Payne 1973相关的简化校正：Ca+0.8×(4−白蛋白)；并非实测离子钙

## 已记录的公式

校正钙 (mg/dL) = 总钙 + 0.8 × (4.0 − 白蛋白（g/dL）).

单位为mmol/L：钙 + 0.02 × (40 − 白蛋白（g/L）).

## 限制与适用人群

Payne 1973论文中的公式来自蛋白水平异常、送检肝功能的样本，白蛋白系数为1，钙以mg/100 mL计，白蛋白以g/100 mL计。本地简化变体采用0.8，需要为该修改提供专门来源。调整钙是一种估计，并非离子钙测定。

## 参考文献

- [Payne RB, Little AJ, Williams RB, Milner JR. Interpretation of serum calcium in patients with abnormal serum proteins. BMJ, 1973.](https://doi.org/10.1136/bmj.4.5893.643)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026

## 已记录的结果

以下信息保留该方法对合成示例的输出，不构成独立的临床验证。

### 1

校正钙处于正常范围（8,5 至 10,5 mg/dL）

该校正为近似值：在危重患者、酸碱失衡或肾脏疾病情况下，请用离子钙确认。


### 2

校正钙偏低（< 8,5 mg/dL）：可能低钙血症

该校正为近似值：在危重患者、酸碱失衡或肾脏疾病情况下，请用离子钙确认。


### 3

校正钙升高（> 10,5 mg/dL）：可能高钙血症

该校正为近似值：在危重患者、酸碱失衡或肾脏疾病情况下，请用离子钙确认。


### 4

校正钙处于正常范围（8,5 至 10,5 mg/dL）

该校正为近似值：在危重患者、酸碱失衡或肾脏疾病情况下，请用离子钙确认。

