# Git 系统学习指南

这是一份完整的 Git 系统学习教程，包含 7 个章节，从基础原理到高级技巧。

## 章节目录

1. **[01 - Git 原理与配置](./01-git原理与配置/Git原理与配置.md)**
   - Git 的设计哲学（分布式、快照模型）
   - Git 对象模型（blob、tree、commit、tag）
   - 三个区域（工作区、暂存区、版本库）
   - 配置体系、.gitignore 规则、Alias 配置

2. **[02 - Git 日常操作命令详解](./02-日常操作命令/Git日常操作命令详解.md)**
   - 初始化与克隆
   - 文件跟踪与提交
   - 状态与差异查看
   - 历史查看
   - 暂存管理（stash）
   - 撤销与恢复
   - 文件操作

3. **[03 - Git 分支与合并详解](./03-分支与合并/Git分支与合并详解.md)**
   - 分支的本质
   - 分支操作（创建、删除、重命名）
   - 合并策略（Fast-forward、三方合并）
   - 冲突解决
   - Rebase 详解
   - merge vs rebase 选型指南

4. **[04 - Git 远程协作详解](./04-远程协作/Git远程协作详解.md)**
   - 远程仓库概念
   - SSH 密钥配置
   - GitHub 仓库创建与关联
   - fetch / pull / push 详解
   - 本地分支与远程分支的跟踪关系
   - Tag 管理
   - Fork + Pull Request 工作流

5. **[05 - Git 历史操控详解](./05-历史操控/Git历史操控详解.md)**
   - git log 进阶（格式化、过滤、搜索）
   - git blame（代码行追溯）
   - git bisect（二分查找 bug）
   - git reflog（恢复误操作）
   - git reset 三种模式
   - git revert（安全撤销）
   - git cherry-pick（摘取提交）

6. **[06 - Git 工作流与提交规范](./06-工作流与规范/Git工作流与提交规范.md)**
   - 主流工作流对比（Git Flow、GitHub Flow、Trunk-based）
   - Conventional Commits 提交规范
   - 工具链（commitizen、commitlint、conventional-changelog）
   - Pull Request 最佳实践
   - 分支命名规范
   - GitHub 合并策略选型

7. **[07 - Git 进阶技巧](./07-进阶技巧/Git进阶技巧.md)**
   - Git Hooks（自动化流程）
   - Git Submodule 与 Subtree（多仓库管理）
   - Git Worktree（并行开发）
   - Sparse Checkout（大仓库优化）
   - .gitattributes（文件属性配置）
   - 性能优化（浅克隆、部分克隆、maintenance）

## 学习建议

1. **按顺序学习**：每章都建立在前面章节的基础上
2. **动手实践**：每章末尾都有实战练习，务必亲手操作
3. **配置别名**：第 1 章的 Alias 配置可以大幅提升工作效率
4. **建立规范**：第 6 章的工作流和提交规范适合团队推行
5. **逐步深化**：初学者重点掌握前 4 章，后续章节视需要选学

## 快速参考

### 最常用的 10 个命令

```bash
git status          # 查看工作区状态
git add .           # 暂存所有变更
git commit -m "msg" # 提交
git push            # 推送到远程
git pull --rebase   # 拉取远程更新
git log --oneline   # 查看提交历史
git branch -av      # 查看分支
git checkout -b     # 创建并切换分支
git merge           # 合并分支
git stash           # 暂存工作区
```

### 常见问题速查

- **怎样撤销已提交的内容？** → 见第 05 章 git reset / git revert
- **怎样解决合并冲突？** → 见第 03 章冲突解决
- **怎样查找引入 bug 的提交？** → 见第 05 章 git bisect
- **怎样规范化提交信息？** → 见第 06 章 Conventional Commits
- **怎样管理大型仓库？** → 见第 07 章 Sparse Checkout 和性能优化

---

**作者说**：这份指南总结了 Git 在实际工程中的最佳实践。掌握这些知识后，你不仅能解决日常遇到的问题，还能在团队中成为 Git 专家，帮助他人解决疑难杂症。
