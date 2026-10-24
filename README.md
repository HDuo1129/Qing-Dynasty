# Qing-Dynasty

This repository is the workflow review for Dong, Jianhao, and Duo on our quantitative history research on the Qing Dynasty.

> **@Dong 提醒：** 用 Codex 写代码时，提交的作者（author）应该是你自己，Codex 只作为 co-author。目前的提交作者都显示为 `Codex`，所以你没有出现在 Contributors 里。请让 Codex 用你本地的 git 身份提交，并在提交信息末尾加上 `Co-authored-by: Codex <codex@users.noreply.github.com>`。具体做法见 [待办事项](docs/project_notes/todo.md) 和 [AGENTS.md](AGENTS.md)。

> **@所有人 提醒：** 每次和 AI（Codex、Claude 等）互动后，都要让 AI 把这次的进展和决定更新到 [AGENTS.md](AGENTS.md) 的 Project memory 部分，并一起提交。这样我们三个人用的不同 AI 能共享同一份记忆。编辑前先 `git pull --ff-only`，避免覆盖别人的记录。

## Files

- [科举之党同伐异](https://hkustgz-my.sharepoint.com/:f:/r/personal/rdu159_connect_hkust-gz_edu_cn/Documents/2026.10.14%20%E7%A7%91%E4%B8%BE%E4%B9%8B%E5%85%9A%E5%90%8C%E4%BC%90%E5%BC%82?d=wb958f47171ec4c66ba576b384b83334e&csf=1&web=1&e=iZsrd4)

## 实证论文项目目录

本地工作目录与本 GitHub 仓库直接对应，代码、说明和文献通过 Git 同步。

| 目录 | 用途 |
| --- | --- |
| `data/raw/` | 原始数据，只保存原件，不手动修改 |
| `data/derived/` | 由代码生成的清洗数据、中间数据和分析样本 |
| `data/additional_data/` | 外部辅助数据 |
| `data/data_sharing/` | 经核验可公开的复现数据 |
| `data/archive/` | 历史数据版本 |
| `code/libs/` | 可复用函数和程序 |
| `code/notebooks/` | 探索分析和研究笔记本 |
| `code/scripts/` | 数据清洗、变量构造和实证分析脚本 |
| `code/workflow/` | 主程序、运行顺序与环境说明 |
| `outputs/figures/` | 论文和汇报图形 |
| `outputs/tables/` | 回归表和描述统计表 |
| `outputs/logs/` | 程序运行日志 |
| `outputs/archive/` | 历史结果 |
| `manuscript/current/` | 当前论文正文及源文件 |
| `manuscript/journal_versions/` | 分期刊投稿版本 |
| `manuscript/comments_and_edits/` | 合作者、审稿意见和修改记录 |
| `manuscript/conferences/` | 会议论文版本 |
| `manuscript/archive/` | 历史稿件 |
| `slides/working/` | 日常工作汇报 |
| `slides/meetings/` | 按日期及会议名称保存的汇报材料 |
| `docs/project_notes/` | 研究日志、会议纪要和待办事项 |
| `docs/decisions/` | 样本、变量和识别策略等重要决策记录 |
| `literature/` | 文献 PDF、文献索引和 BibTeX |
| `literature/notes/` | 文献阅读笔记 |

### 日常使用

1. 新数据放入相应数据目录，并在 [数据说明](data/README.md) 登记来源、取得日期、权限和处理程序。
2. 按“导入与清洗 → 构造变量 → 描述统计 → 基准回归 → 稳健性与机制 → 图表导出”组织代码；确定软件和数据后，在 `code/workflow/` 记录可复现的运行入口。
3. 当前稿件放在 `manuscript/current/`，图表由代码输出到 `outputs/`；每次会议使用 `slides/meetings/YYYY-MM-DD_event/` 独立目录。
4. 提交代码、说明、稿件和指定文献。数据文件默认不进入 Git，需公开的数据经核验后再明确添加。

### Git 同步

远程仓库：<https://github.com/HDuo1129/Qing-Dynasty>，默认分支：`main`。

请从本项目根目录执行 Git 命令；本目录有独立的 `.git/`。

```bash
git pull --ff-only
git status
git add <本次需要同步的文件>
git commit -m "Describe the research update"
git push origin main
```

空目录通过 `.gitkeep` 在 GitHub 中保留。原有共享资料链接保留在上方。
