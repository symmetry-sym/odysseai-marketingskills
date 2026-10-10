# 营销技能工具箱｜Codex 安装包

此仓库提供 `marketingskills` Codex Skill。入口会根据任务选择营销模块；模块指南、参考资料和示例均在 `marketingskills/references/` 中，需连同入口一起安装。

## 安装

在 Codex 中发送：

```text
请用 skill-installer 安装 GitHub 仓库 symmetry-sym/odysseai-marketingskills 中的 marketingskills 目录，技能名设为 marketingskills。
请安装整个目录，不要只下载 SKILL.md。安装后实际读取 SKILL.md，并检查 references/module-index.md 和索引列出的 50 个模块 guide.md 均存在；报告实际安装路径和缺失项。只报告实际检查到的结果。
```

脚本安装方式：

```bash
python3 "$HOME/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py" \
  --repo symmetry-sym/odysseai-marketingskills \
  --path marketingskills \
  --name marketingskills
```

安装完成后，在下一轮对话中调用 `marketingskills`。如果 Codex 当前窗口还没显示新技能，重新打开菜单或重启 Codex。

## 使用

```text
使用 marketingskills：

业务/产品：
目标客户：
当前阶段：
营销目标：
主要渠道：
已有材料或数据：
希望交付：
限制条件：
```

入口会先读模块索引，选一个最匹配的主模块；确实跨领域时才组合其他模块。缺少的信息应标成假设或待确认项。起草方案不等于已经发布广告、发送邮件或完成付费操作。

## 来源与许可

本包保留本机安装版的 281 个文件和 50 个内部模块，另补许可证与来源说明。上游来源为 [coreyhaines31/marketingskills](https://github.com/coreyhaines31/marketingskills)，许可证为 MIT；完整许可文本与打包说明见 `marketingskills/LICENSE`、`marketingskills/NOTICE.md`。本机副本没有 Git 元数据，无法从目录确认精确上游提交号。
