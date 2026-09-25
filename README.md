# skill-lifecycle-manager

一套贯穿 skill 生老病死的元认知闭环。它不干具体业务，只做五件事：**触发判断 → 申请建立 → 分层 → 脚本化迁移 → 使用后迭代**。每一步的关键是「**先申请、后执行**」——绝不自动落地，人类始终是裁决者。

## 环境依赖

- 操作系统：Windows
- 运行时：无（纯指令型 skill，由 agent 直接执行）
- 第三方软件：无（仅依赖系统自带的 PowerShell / 标准库）

## 目录结构

    skill-lifecycle-manager/
    ├── SKILL.md    技能入口与工作流
    ├── evals.yaml

## 安装

    # GitHub
    git clone https://github.com/hpsks416/skill-lifecycle-manager.git "$env:USERPROFILE\.dsh\skills\skill-lifecycle-manager"
    # 或 Gitee（国内直连）
    git clone https://gitee.com/hpsks416/skill-lifecycle-manager.git "$env:USERPROFILE\.dsh\skills\skill-lifecycle-manager"

克隆后 DSH 自动重新发现，无需构建。

## License

MIT License. See [LICENSE](LICENSE).
