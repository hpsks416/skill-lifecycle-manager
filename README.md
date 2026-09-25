# skill-lifecycle-manager

Manage the full lifecycle of skills with metacognition — after a task or conversation finishes, judge whether it is worth codifying into a skill, ask the user before creating, split it into the right layer, migrate scriptable parts to local scripts to cut token use, and after a skill is used judge whether it needs iteration. Use when a complex task wraps up, the user asks "要不要做成 skill", or a skill just got used and may need improving. Not for single-step tasks or one-off queries.

## 这是什么

DSH（DeepSeek Harness）skill —— 一个可由 AI agent 按需自动加载的能力单元。克隆到 skill 目录后，DSH 会依据上方描述自动发现并触发它，无需构建。

## 安装

最简单：用 [dsh-config](https://github.com/hpsks416/dsh-config) 的一键脚本 `install.ps1` 批量安装全部 skill。单个安装：

    # GitHub
    git clone https://github.com/hpsks416/skill-lifecycle-manager.git "$env:USERPROFILE\.dsh\skills\skill-lifecycle-manager"
    # 或 Gitee（国内直连更快）
    git clone https://gitee.com/hpsks416/skill-lifecycle-manager.git "$env:USERPROFILE\.dsh\skills\skill-lifecycle-manager"

克隆后 DSH 会自动重新发现，无需重启。更新用：

    git -C "$env:USERPROFILE\.dsh\skills\skill-lifecycle-manager" pull

## 目录结构

    skill-lifecycle-manager/
    ├── SKILL.md    技能入口与工作流
    ├── evals.yaml

## 依赖

无运行时依赖，纯指令型 skill（由 agent 直接执行 Markdown 工作流）。

## License

MIT License. See [LICENSE](LICENSE).
