# 04 产品说明与 FAQ

**检查日期：2026-10-11（America/Chicago）。**

## 适用条件

适合把已批准的图纸、包装资料和规格整理成英文产品卡与 FAQ。需要能够逐条追溯的参数，并知道哪些材料可以上传。

没有证书、测试或内尺寸资料时，不生成认证、承重和容积声明。产品图片可以辅助核对外观，不能替代正式规格。

## 准备输入

填写 [产品事实表](../templates/product-facts.md)。每条事实标明来源编号和版本；图纸与销售资料矛盾时，先由产品负责人确认。

## 操作流程

1. 按型号整理材料，拆出材质、用途、外/内尺寸、包装、MOQ 和未知字段。
2. 可以直接粘贴已确认字段；使用文件上传时先核对账号允许的格式与资料范围。
3. 让 AI 先提取参数并标来源，再生成产品卡。逐条检查抽取结果后再用其写作。
4. 输出适用用途、事实型说明、参数表与 FAQ；“利益点”也要能对应实际事实。
5. 将客户可读内容与内部缺失清单分开。公开稿不留下内部底价、批注或未经确认的技术承诺。
6. 产品负责人复核后再导出或发布，并保留资料版本。

## 可复制提示词

```text
请根据以下虚构产品事实生成英文产品资料草稿。
输出：简短英文产品卡；三条 FAQ；内部“声明/来源/状态”核对表。

P01：FR-10，棕色瓦楞纸板折叠收纳盒，非食品干货整理用途。
P02：外尺寸 400 × 300 × 200 mm；未提供内尺寸、承重和容积。
P03：每件配纸套，20 件/箱，MOQ 500 件。
P04：认证、定制工艺、库存与交期均未知。

不能增加认证、环保标签、食品接触许可、承重、容量、耐水性或保修。
不能从外尺寸计算并宣称内部容量。
FAQ 回答包装与 MOQ；交期问题说明需要核对。
没有来源的字段放入内部待确认清单，不写入产品优势。
```

## 教学示例：客户版资料与内部表

以下是预先编写的虚构教学期望输出，未上传文件到 AI 平台测试。

```text
FR-10 Folding Storage Box

A brown corrugated-cardboard folding storage box for organizing
non-food dry items.

Specifications
- External dimensions: 400 × 300 × 200 mm
- Packaging: one paper sleeve per unit, 20 units per carton
- MOQ: 500 units

FAQ
Q: How is the product packed?
A: Each unit has a paper sleeve. A carton contains 20 units.
Q: What is the minimum order quantity?
A: The MOQ is 500 units.
Q: What is the lead time?
A: Lead time needs to be confirmed for the order.
```

| 声明 | 来源 | 状态 |
| --- | --- | --- |
| 材质、颜色与用途 | P01 | 输入已确认 |
| 外尺寸，不是内尺寸 | P02 | 输入已确认 |
| 包装与 MOQ | P03 | 输入已确认 |
| 容积、承重、认证与交期 | P02/P04 | 未知，不做产品保证 |

## 验收与异常处理

| 检查用例 | 期望结果 |
| --- | --- |
| 只有外尺寸 | 不新增“24 L 内部容量” |
| 没有认证文件 | 不出现认证标签或认证编号 |
| 图纸与包装表显示不同型号 | 暂停生成，先确认型号与版本 |
| 上传工具无法提取扫描参数 | 转人工核对，不能把空字段当作零 |

## 官方资源、费用与补充教程

- [ChatGPT 文件上传](https://help.openai.com/en/articles/8555545-uploading-files-and-audio-to-chatgpt)：从文档提取、对比产品字段与报价说明。
- [ChatGPT 提示词最佳实践](https://help.openai.com/en/articles/10032626-prompt-engineering-best-practices-for-chatgpt)：明确任务、背景、语气，逐轮调整提示词。

文件能力、单个文件与上传次数限制受套餐、模型、地区和工作区设置影响。本次未确认个人账号可用额度；没有上传功能时可人工复制少量已批准字段，保留相同复核步骤。

- [TOOLBBS：ChatGPT 使用教程](https://www.toolbbs.com/sites/2041.html)：已核验产品描述、文件分析及原文复核段落，适合补充理解资料准备。

[返回专题首页](../README.md)
