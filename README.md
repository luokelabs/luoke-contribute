# 一起来做螺壳

螺壳（luoke）是一组只在你自己的 Mac 上跑的 AI 应用：模型、记忆、你交给它们的东西，都留在这台电脑里。

这个仓库是参与螺壳的入口。先看你想做哪一种：

| 你想 | 去哪 |
|---|---|
| 说说想让本地 AI 帮你做什么 | [许个愿](#许个愿) |
| 给已经有的应用报问题、改代码 | [给已有的项目出力](#给已有的项目出力)：直接去那个项目的仓库 |
| 做一个螺壳里还没有的东西 | [做一个新的](#做一个新的)：在这里申请 |

[English](#english)

## 许个愿

不会写代码也没关系。到 [Discussions → Ideas](https://github.com/luokelabs/luoke-contribute/discussions/categories/ideas) 开一个帖子：

- 一个帖子只说一件事，用大白话写清楚：在什么时候、想让它帮你做什么。
- 看到喜欢的愿望，点 ⬆️ 投一票（没有 GitHub 账号的话，在官网许愿墙上点 ❤️ 也算）。票多的，我们先做。
- 官网的许愿墙会挑一部分放上去：[luoke.ai/contribute](https://luoke.ai/contribute)。

## 给已有的项目出力

已经有的应用，各有自己的仓库。报问题、提想法、改代码，**直接去那个仓库开 issue 或 PR**，照它自己的 `CONTRIBUTING.md` 来：

| 项目 | 仓库 | 是什么 |
|---|---|---|
| 邮件助手 | [luoke-mail](https://github.com/luokelabs/luoke-mail) | 用本机模型整理整个邮箱，邮件不出你的 Mac |
| 输入法 | [luoke-ime](https://github.com/luokelabs/luoke-ime) | 本机模型按前文挑词的 macOS 中文输入法，引擎可插拔 |
| 螺壳 | [luoke-core](https://github.com/luokelabs/luoke-core) | 管模型、引擎、内存和功耗，给各应用派任务，也是安装器 |
| 螺壳记忆 | [luoke-mem](https://github.com/luokelabs/luoke-mem) | 各应用共用、只在本机的记忆，每条都有依据、能改能删 |

- **改代码先开 issue**，说清楚要解决什么、打算怎么改，商量好再提 PR。
- **写输入法引擎不用改仓库**：照 [写一个引擎](https://github.com/luokelabs/luoke-ime/blob/main/docs/写引擎.md) 写好，放进本机就能用。想让大家都用上，到 [luoke-ime](https://github.com/luokelabs/luoke-ime/issues) 开 issue 说一声。
- **你机器上的实测**：到 [luoke-core](https://github.com/luokelabs/luoke-core/issues) 开 issue，写清芯片、内存和 macOS 版本，补上我们手上没有的机型。
- issue 和 PR 里不要贴真实的邮件、打过的字、记忆；需要例子就编一个。
- 安全问题不要开公开 issue，见各仓库的 `SECURITY.md`。

## 做一个新的

做了一个螺壳里还没有的本地 AI 小工具，或者想做一个，在[这个仓库开 issue](https://github.com/luokelabs/luoke-contribute/issues/new/choose) 申请：

1. **说清楚它是什么**：做什么、给谁用、怎么跑、用户的数据会去哪；要用螺壳的模型、记忆哪些能力。已经有代码的，附上仓库链接。
2. **我们一起看一遍**：照下面几条对一对，有问题在 issue 里聊。
3. **合适，就立项**：一起商量放进螺壳的方式（单独一个仓库，或者并进已有的项目），署上你的名字。

还没想清楚怎么做、只是想要一个，去 [许个愿](#许个愿)。

## 我们一直守着的几件事

不管是改已有的项目还是做新的，都照这几条：

- 东西只在本机跑，不把用户的东西传出去，哪怕只是一点统计。
- 模型全机只有一份，要用就经螺壳，不自己再装一份。
- 改东西、发东西、删东西之前，都要先问用户。
- 密码、验证码这类秘密不碰。

## 说话的规矩

友好、就事论事。广告、人身攻击、泄露别人隐私的内容会被删掉。

---

## English

Luoke is a set of AI apps that run only on your own Mac. This repo is where you take part:

- **Make a wish** — post in [Discussions → Ideas](https://github.com/luokelabs/luoke-contribute/discussions/categories/ideas) what you'd like local AI to do for you, and upvote the ones you like (likes on the luoke.ai wish wall count too). The most-voted get built first.
- **Help an existing project** — go straight to its repo and follow its `CONTRIBUTING.md`: [luoke-mail](https://github.com/luokelabs/luoke-mail) (Mail), [luoke-ime](https://github.com/luokelabs/luoke-ime) (Chinese input method), [luoke-core](https://github.com/luokelabs/luoke-core) (the hub), [luoke-mem](https://github.com/luokelabs/luoke-mem) (memory). Open an issue before sending a pull request. Benchmarks from your Mac go to luoke-core.
- **Build something new** — open an [issue here](https://github.com/luokelabs/luoke-contribute/issues/new/choose) describing what it does, who it's for, how it runs and where user data goes. We review it together against the rules above (local only, one shared model through Luoke, ask before acting, no secrets), and if it fits, we decide together how it joins Luoke, with your name on it.
