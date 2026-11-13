# 来源、取舍与使用边界

## 用户提供材料

本候选基于用户授权审阅的四份本机材料进行原创压缩：

- `双AI协作部署模板.md`
- `后端架构设计标准.md`
- `后端架构验收标准.md`
- `research-evidence-core.zip`

原始材料的作者、许可证和再分发条件尚未确认。本候选不复制原文、代码或固定模板，只提炼通用思想供用户个人项目使用；若要公开发布，应先取得作者许可并重新做相似性审查。

## 选择性吸收

保留：

- 主张级证据、事实/推断分离、反证和推翻条件；
- 数据健康度和未验证状态；
- 业务边界优先、框架复用、最小纵向切片；
- Owner回报、独立审查和最小交接。

改写：

- 固定“双AI”改为通用角色；
- 全量后端清单改为适用性与风险分级；
- “全部通过才开发”改为硬门禁＋最小验证切片；
- 每动作留档改为只记录长期有价值的决定和交接。

不采用：

- 第二套规则优先级或镜像权威目录；
- 固定某模型为永恒审查者/实现者；
- 对所有项目强制数据库、权限占位或十一种接口场景；
- 以结构校验脚本证明来源真实或结论正确；
- 原ZIP中的 `__pycache__` 和未知许可脚本。

## GitHub/公开方案对照（2026-08-08）

仅用于结构和取舍，没有复制代码或文本：

- [anthropics/skills](https://github.com/anthropics/skills)：验证自包含目录、`SKILL.md` 元数据和渐进式资源结构；仓库包含混合许可内容，因此未复用正文。
- [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills)：参考按生命周期拆分 Skill 和质量门禁的思路；未引入其整套命令或共享引用。
- [obra/superpowers](https://github.com/obra/superpowers)：对照规格→计划→构建→验证的工作流；本候选拒绝自动引入其子Agent或TDD体系。
- [architecture-decision-record/architecture-decision-record](https://github.com/architecture-decision-record/architecture-decision-record)：借鉴重要决定记录背景与后果的概念；未复制任何具体模板。
- [commonal/research-evidence-agent](https://github.com/commonal/research-evidence-agent)：对照事实、推理和待验证假设分层；其完整软件架构不适合本轻量 Skill。

GitHub 元数据和许可证可能变化；正式再分发前应重新核对具体文件许可证、提交版本和引用范围。

## 与现有治理的关系

本候选不替代：

- 全局或项目 `AGENTS.md`；
- 网站交付、Payload、Eli或其他专项Skill；
- 生产、部署、迁移、删除、付款、权限或外写授权；
- 真实浏览器、设备、生产或用户验收。

如果本候选与更高优先级规则冲突，停止使用冲突条款并报告，不修改上位规则。
