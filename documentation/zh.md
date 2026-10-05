<!-- ELUCENIA technical documentation · wells-tep · zh · no clinical/professional/rights approval -->

# Wells 评分（肺栓塞）

[条件、来源与许可](https://elucenia.org/zh/tools/wells-tep)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### 深静脉血栓的临床体征

`tvp`

### 肺栓塞是最可能的诊断

`alt`

### 心率 \> 100 bpm

`fc`

### 制动 ≥ 3 天或过去 4 周内手术

`imob`

### 既往深静脉血栓或肺栓塞

`prev`

### 咯血

`hemo`

### 活动性癌症（过去 6 个月内治疗或姑息治疗）

`cancer`

## 方法版本

Wells PE 2000：7项加权因素；2级和3级分类分开

## 已记录的公式

分值相加：DVT体征3 · PE更可能3 · 心率\>100计1.5 · 制动/手术1.5 · 既往DVT/PE 1.5 · 咯血1 · 癌症1。

## 限制与适用人群

肺栓塞Wells评分在临床疑似病例中研究，所用策略结合评分与D-二聚体。二级和三级分类具有不同阈值；低评分或肺栓塞可能性不大并不等同于无肺栓塞。D-二聚体检测法和应用标准须与所用诊断方案一致。

## 参考文献

- [Wells PS et al. Derivation of a simple clinical model to categorize patients probability of pulmonary embolism. Thromb Haemost, 2000.](https://doi.org/10.1055/s-0037-1613830)

- [Konstantinides SV et al. 2019 ESC Guidelines for the diagnosis and management of acute pulmonary embolism. Eur Heart J, 2020.](https://doi.org/10.1093/eurheartj/ehz405)

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
