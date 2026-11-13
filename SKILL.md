---
name: evidence-gated-project-workflow
description: Applies evidence gates, project-fit checks, adversarial review, and explicit acceptance states to consequential research, backend architecture, and multi-agent handoffs. Use when the user asks for 调研审查、证据审查、市场/行业/公司研究、后端架构设计、架构验收、Owner派单、独立验收、多AI协作、successor交接, or when an important project decision needs traceable evidence and failure conditions.
---

# 证据门禁项目工作流

## 目标

把重要判断、后端架构和协作交接收敛为可追溯、可反证、可验收的最小闭环。它补充而不覆盖平台、全局 `AGENTS.md`、项目规则、授权和专项 Skill。

## 不适用

- 普通问答、翻译、轻微文案和低风险机械修改。
- 用文档清单替代真实执行、测试、浏览器、生产或用户验收。
- 以本 Skill 扩大部署、删除、迁移、权限、付款或外部写入授权。
- 用固定目录、固定技术栈或固定 AI 品牌替代项目事实。

## 快速路由

只读取本任务需要的一个参考文件；跨域任务才组合读取：

- 研究、报告、方案证据审查：读 [research-evidence.md](references/research-evidence.md)。
- 后端选型、骨架、接口或架构验收：读 [backend-architecture.md](references/backend-architecture.md)。
- Owner、执行者、审查者之间交接：读 [collaboration-handoff.md](references/collaboration-handoff.md)。
- 需要了解本候选的来源和取舍：读 [source-notes.md](references/source-notes.md)。

## 通用工作流

1. **确认对象**：身份、版本、目的、受众、时间、范围、授权和验收人。
2. **判断适用性**：逐项标记 `适用 / 不适用 / 待确认`；不适用必须说明原因。
3. **建立事实底座**：区分观察事实、计算、推断、建议、假设和未知。
4. **形成最小方案**：只保留实现目标所需的规则、模块和证据。
5. **对抗式检查**：寻找越权、证据替代、隐藏冲突、过度设计、静默降级和不可逆失败。
6. **执行或审查**：Owner 负责实际结果；独立审查者不得用作者自检替代。
7. **门禁收口**：只使用 `通过 / 条件通过 / 未通过 / 未验证`，并绑定证据和下一步。

## 最小输出契约

```text
结论：
对象与范围：
适用/不适用项：
事实与证据：
关键判断及置信度：
反证与失败方式：
验证结果：
残余风险：
Owner / 下一步 / 到期条件：
```

## 硬门禁

- 对象、版本或范围不清且会改变结论。
- 核心判断无可定位证据，或把推断写成事实。
- 安全、隐私、权限、数据完整性或不可逆动作未处理。
- 关键验证未执行却声称通过。
- 需要独立验收却只有作者自检。
- 规则与当前项目事实冲突，仍机械套用模板。

命中硬门禁时停止给出绿色结论；输出缺口、影响、责任人和补证方式。

## 使用原则

- 目录多、文档多、Agent 多不代表质量高。
- 清单是提醒，不是证据；工具或 Agent 自述不是最终验收。
- 条件通过必须写明 Owner、期限、补偿控制、复验方式和失效条件。
- 重要决定记录背景、候选方案、取舍、后果和回滚/退出路径。
- 只在产生长期复用价值时留档，避免每个动作都生成文档。
- 已有、可定位且与当前版本/输入/环境匹配的有效产物可复用；不要求每轮重产。
- 非文件交付不强制落盘。使用全局状态词报告任务状态，验收结论单列为 `通过 / 条件通过 / 未通过 / 未验证`。
- 执行 Owner 生成验证证据；PMO 审核原始证据、范围和时效，不以自述代替证据，也不因职责要求亲自重跑。
