# 来源与检查记录

**检查日期：2026-10-11（America/Chicago）。**

## 仓库与内容范围

- GitHub CLI 与已连接应用的账号均为 `zoow1388-svg`，本次登录有效。
- 创建前检查了账号下现有仓库名称与说明，并读取综合仓库 README。没有 `ai-for-export-business` 同名仓库。
- 综合仓库在检查时的 main 提交为 `bb8f72bdf8782ec3536456910de2d5c40a64c38b`，内容为六类资源目录。本专题只在 README 以目录入口引用，不复制其条目。
- 新专题包含六份业务指南、四份模板、七组提示词、十四个官方来源和三篇中文教程；未修改综合仓库或其他项目。

## 链接检查方法

1. 用网页工具逐项打开官方来源与三个中文教程，阅读与指南有关的正文，核对功能、操作步骤及可确认的限制。
2. 本机对 19 个不同外部地址各执行一次 HTTP GET，跟随正常重定向，不自动重试、不登录网站。
3. 19 个地址由 14 个官方来源、3 个中文教程、1 个品牌主页和 1 个综合目录入口组成。
4. 本机结果：**13 个 HTTP 200，6 个 HTTP 403**。六个 403 地址为 O01–O06；网页工具均返回了相关官方正文。本机普通浏览器访问与 403 原因未确认，不能据此宣称本机访问问题已解决。
5. HTTP 状态与正文核验是不同证据。200 不表示业务步骤已运行成功；网页工具读取正文也不表示个人账号已开通功能。
6. OpenAI 搜索、上传与数据控制帮助页发生标题地址调整，采用已核实的当前正式地址。n8n 人工审批页面按当前官方文档索引找到新路径，不照搬旧版教程的页面路径。

## 官方来源

| 编号 | 官方页面 | 本机 GET | 已阅读内容与边界 |
| --- | --- | --- | --- |
| O01 | [ChatGPT 提示词最佳实践](https://help.openai.com/en/articles/10032626-prompt-engineering-best-practices-for-chatgpt) | HTTP 403 | 已读取官方说明，覆盖清楚具体、提供背景、迭代与语气。 |
| O02 | [ChatGPT 搜索与来源核对](https://help.openai.com/en/articles/9237897-searching-the-web-with-chatgpt) | HTTP 403 | 官方说明搜索入口、引用和搜索结果可能不完整或错误。 |
| O03 | [ChatGPT 文件上传](https://help.openai.com/en/articles/8555545-uploading-files-and-audio-to-chatgpt) | HTTP 403 | 已读取文件上传、提取、转换及套餐/地区限制；未把上传额度写成固定保证。 |
| O04 | [ChatGPT 数据控制](https://help.openai.com/en/articles/7730893-data-controls-in-chatgpt) | HTTP 403 | 官方说明关闭训练选项不等于删除聊天记录；临时聊天也有保留边界。 |
| O05 | [DeepL 文件翻译](https://support.deepl.com/hc/en-us/articles/360020569480-Translate-files-with-DeepL-file-translation) | HTTP 403 | 官方给出选择文件、源/目标语言、翻译和下载流程。 |
| O06 | [DeepL 术语表](https://support.deepl.com/hc/en-us/articles/360021634540-About-the-glossary) | HTTP 403 | 官方说明词条、语言对、平台和存储差异；未假设每个账号功能相同。 |
| O07 | [DeepL 套餐与限制](https://www.deepl.com/en/pro) | HTTP 200 | 已读取套餐比较；具体地区实付价格、个人可用额度本次未确认。 |
| O08 | [Dify 关联知识库与引用](https://docs.dify.ai/en/cloud/use-dify/knowledge/integrate-knowledge-within-application) | HTTP 200 | 已读取关联知识库、Citation and Attribution、Debug and Preview 的操作说明。 |
| O09 | [Dify 检索测试](https://docs.dify.ai/en/cloud/use-dify/knowledge/test-retrieval) | HTTP 200 | 官方说明 Retrieval Testing，以及测试中的设置只在本次测试生效。 |
| O10 | [Dify 套餐与额度](https://dify.ai/pricing) | HTTP 200 | 页面提供免费 Sandbox 和付费方案；模型调用、存储和请求限制需核对。 |
| O11 | [n8n 工具调用人工审批](https://docs.n8n.io/build/integrate-ai/ai-examples/human-in-the-loop-for-tools) | HTTP 200 | 官方当前页面说明 Tools、Human review、Approve/Deny；没有执行工作流。 |
| O12 | [n8n 套餐与执行额度](https://n8n.io/pricing/) | HTTP 200 | 已读取按工作流执行量计费及计划限制；本次未确认实际购买价格。 |
| O13 | [ICC Incoterms® 2020](https://iccwbo.org/business-solutions/incoterms-rules/incoterms-2020/) | HTTP 200 | 官方发布方页面说明贸易术语及出版物；未复制付费规则全文。 |
| O14 | [英国 Companies House 查询](https://find-and-update.company-information.service.gov.uk/) | HTTP 200 | 官方登记搜索入口可访问；页面提醒登记信息准确性并非由该机构逐项核查。 |

上述为官方来源数量，不是十四种不同 AI 产品。引用文档用于说明工具能力和核对入口；业务步骤、提示词与教学示例由本项目独立编写。

## TOOLBBS 中文教程

| 编号 | 已核验教程 | 本机 GET | 与专题有关的内容 |
| --- | --- | --- | --- |
| T01 | [TOOLBBS：ChatGPT 使用教程](https://www.toolbbs.com/sites/2041.html) | HTTP 200 | 已核对外贸邮件、产品描述、市场调研与原文复核段落；版本和价格不作为依据。 |
| T02 | [TOOLBBS：Dify 知识库与客服教程](https://www.toolbbs.com/sites/2121.html) | HTTP 200 | 已读取知识库、聊天应用、客服及新手教程相关段落。 |
| T03 | [TOOLBBS：n8n 邮件分类教程](https://www.toolbbs.com/sites/2127.html) | HTTP 200 | 已核对触发器、AI 分类、分支、测试与人工复核内容；不采用旧部署路径。 |

教程中的历史价格、型号名称、部署命令和商业效果没有作为本专题的当前事实。资料能力以对应官方页面为准，所有教程保持真实地址。

维护方首页与综合目录入口本次均返回 HTTP 200；它们只在 README 中分别作为品牌和目录链接。

## 示例与验收的含义

- FR-10、示例客户 A、P01–P04、S01–S03、K01–K04 和 Q-DEMO-001 都是教学资料，不代表真实客户、产品、网页、知识条目或订单。
- 六份指南写明适用条件、输入、步骤、提示词、期望输出和异常处理；客户研究同时提供在线任务与离线虚构练习。
- 指南中的验收表是供读者实测时使用的条件，不是已经完成的平台测试报告。
- 报价采用单一 USD 币种，价格与折扣是虚构的已审批输入；3,765.00 USD 是已知费用小计，不含未确认的运费、保险和税费。
- 官网使用资格、具体地区实付价格、个人额度和数据保留设置本次未登录核对，指南已注明未知。
- 本次没有执行 AI 平台操作、工作流、真实企业信用调查、客户邮件发送、真实报价、客服部署或订单/退款动作。

## 读者复核方法

1. 从 README 打开每份指南，检查适用条件与手工路径。
2. 用虚构输入在获准工具中运行提示词，按该指南的验收表检查结果并记录平台、日期和模型。
3. 金额由独立计算方式复核；来源与数值矛盾时先补资料再生成。
4. 检索有出处仍需核对生成答复；转人工建议不等于已完成工单交接。
5. 不要求部署服务器。使用真实系统、接入自动化或对外使用结果时，应走团队已有业务流程。

这是文档项目，没有运行依赖；构建、应用启动和平台自动化运行测试均未执行。

## 本次提交前实际检查

| 检查 | 结果 |
| --- | --- |
| 文档结构与数量 | 六份指南、四份模板、七组提示词、十四个官方来源和三篇中文教程一致。 |
| 文档链接与格式 | 仓库内相对链接存在；外链与核验输入一致；UTF-8、标题和围栏检查通过。 |
| GitHub Markdown 预览 | 十三份文档通过官方 Markdown 渲染接口，表格与文本示例成功返回。 |
| 报价独立计算 | 十进制计算得到货值 3,800.00、折扣 95.00、折后 3,705.00、已知费用小计 3,765.00 USD；50 箱。 |
| 内容差异 | 已阅读新增文档差异；十三个文件全部属于本专题；综合仓库文件哈希与原提交一致。 |
| 示例标识 | 检查发现翻译指南缺少独立虚构标识，已补充后通过；未降低检查标准。 |
| 密钥与临时文件 | 未发现常见密钥格式；临时检查脚本未进入仓库；没有运行代码或依赖改动。 |
