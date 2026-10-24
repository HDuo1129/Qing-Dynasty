# 待办事项

## Dong

- [ ] 用 Codex 提交时，把自己设为主要作者，Codex 只作为 co-author（2026-10-24 提出）

  现在仓库里由 Codex 推送的提交，作者都是 `Codex <codex@users.noreply.github.com>`，所以 GitHub 把贡献算给了 Codex，你没有出现在 Contributors 里。

  1. 本地设置你的提交身份，邮箱要和你 GitHub 账号绑定的邮箱一致：
     ```bash
     git config user.name "你的名字"
     git config user.email "你在 GitHub 绑定的邮箱"
     ```
  2. 让 Codex 提交时不要改作者，用上面这个本地身份，并在提交信息最后空一行加上：
     ```
     Co-authored-by: Codex <codex@users.noreply.github.com>
     ```
     仓库根目录的 `AGENTS.md` 已经写了这条规则，Codex 会自动读取。
  3. 之后的提交在 GitHub 上会显示你是作者、Codex 是共同作者，你也会出现在 Contributors 列表中。
  4. 确认没问题后，删除 README 顶部的提醒，并勾选本条。
