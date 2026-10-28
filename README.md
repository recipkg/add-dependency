# add-dependency

为 Recipkg 配方声明并集成一个具体依赖，核对递归关系、接口、来源和固定版本。用于添加依赖、引入现有软件配方或接入 GitHub 配方仓库。

Read [SKILL.md](SKILL.md) for the workflow and linked resources. This is the canonical standalone skill repository used by [Recipkg](https://github.com/recipkg/recipkg).

## Use as a project submodule

```sh
git submodule add https://github.com/recipkg/add-dependency.git .agents/skills/add-dependency
git submodule update --init --recursive
```

Keep the same repository across projects. Review upstream changes and local work before checking out a new commit, then explicitly commit the consumer gitlink. Do not copy and hand-maintain a second skill or overwrite custom modifications.

This repository is also a Markdown-only Recipkg skill recipe: validate with `recipkg check .`, then pack it outside this directory. [License](LICENSE.md).

## 中文

本仓库只维护 `add-dependency` 技能。不同项目应把此同一仓库作为固定提交的 Git 子模块引用，不复制技能正文。修改先回本仓库，再更新项目指针；注意保护本地改动。技能入口与说明见 [SKILL.md](SKILL.md)。
