# git_practice

信息安全专业的学习仓库：课程作业、CTF 练习、每周反思和专业笔记都在这里沉淀。

远程仓库：https://github.com/LLz-oo/git_practice.gitGitHub 打开仓库默认显示 `main` 分支，它代表"当前最新、可阅读/可运行"的版本。

## 目录导航

| 目录 | 用途 |
| --- | --- |
| `weekly/` | 每周反思，文件按 ISO 周命名，如 `2026-W48.md` |
| `homework/` | 课程作业，每次作业一个文件夹 |
| `ctf/` | CTF writeup、解题脚本、常用 payload 速查 |
| `courses/` | 专业课笔记：密码学、网络、操作系统等 |
| `labs/` | 靶场与实验进度记录 |
| `vuln-research/` | CVE 与漏洞复现档案 |
| `reading/` | 论文与书籍读书笔记 |
| `tools/` | 自己写的工具脚本 |
| `ETHICS.md` | 练习边界与红线，动手前先读 |

## 约定

- 一次提交只做一件事，提交信息用前缀：`hw:` / `ctf:` / `weekly:` / `notes:` / `fix:` / `docs:`。
- 每周日复制 `weekly/TEMPLATE.md` 写周报并提交，年末用 `git log --oneline` 回顾成长曲线。
- 编译产物不要提交，见 `.gitignore`。
- 只在授权环境里做安全测试，见 `ETHICS.md`。

## 常用命令

```bash
git status                                   # 看改了哪些文件
git add .                                    # 暂存全部改动
git commit -m "weekly: 完成 2026-W48 周报"   # 提交一个快照
git push -u origin main                      # 首次推送，之后直接 git push
git pull                                     # 拉取远端更新
```

改错了想撤销未提交的修改：`git checkout -- 文件名`；看历史：`git log --oneline`。
