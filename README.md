# 账号注册与收码 Skill

面向 Codex 的注册协作技能，整理 Devin 与 TypeSafe 两条历史流程的决策经验：核对实际页面、准确筛选本次验证码、返回原标签页、识别已有登录会话，以及提交结果不明时安全恢复。

## 安装与调用

将本仓库的 `account-registration` 文件夹放入 `$CODEX_HOME/skills/`；未设置 CODEX_HOME 时放入 `~/.codex/skills/`。在新对话中调用：

> 使用 $account-registration 帮我完成这个网站的授权注册，先验证一个账号。

入口：[SKILL.md](account-registration/SKILL.md)。引用资料位于 `account-registration/references/`。

## 能力与边界

这是指导 AI 决策的技能，不是独立运行的注册机，不附带账号、密码、Cookie、API 密钥或绕过验证的方法。它仍需要可用的浏览器工具或适用的官方接口，以及用户授权。历史中未完成的真实验收明确保留为未验证。

已通过技能结构及引用链接检查；这不等于两个网站的完整注册流程均已通过当前版本实测。
