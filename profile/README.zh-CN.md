<div align="center">

<img src="https://download.alianblank.com/gameframex/gameframex_logo_320.png" alt="Game Frame X Logo" width="160" />

# GameFrameX

[![License](https://img.shields.io/badge/license-blue.svg)](../LICENSE.md)
[![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://gameframex.doc.alianblank.com)

[![Discord](https://img.shields.io/badge/-5865F2?logo=discord&logoColor=white)](https://discord.gg/VDWUjWMDw9)
[![GitHub](https://img.shields.io/badge/-181717?logo=github&logoColor=white)](https://github.com/GameFrameX/gameframex)
[![Bilibili](https://img.shields.io/badge/-00A1D6?logo=bilibili&logoColor=white)](https://www.bilibili.com/video/BV1yrpeepEn7)
[![Gitee](https://img.shields.io/badge/-C71D23?logo=gitee&logoColor=white)](https://gitee.com/GameFrameX/gameframex)

独立游戏前后端一体化解决方案 · 独立游戏开发者的圆梦大使

<br />

[文档](https://gameframex.doc.alianblank.com) · [快速开始](#快速开始) · QQ群: 467608841 / 233840761

<br />

[English](README.md) | **简体中文** | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

</div>

## 项目简介

一个人做联网游戏，要扛的远不止玩法：选客户端引擎、写服务器、选数据库、搭配置表流程、配发布 CI——上线之后，还得有个后台看玩家数据。单拎出来没有一件难；难的是每一件都落在你一个人头上。

GameFrameX 一次性把这些都给你：多引擎客户端、多进程服务器、双数据库、配置表工具、网络协议、一体化后台、三平台 CI。你只管专注玩法，剩下的，框架已经组装好了。

游戏引擎延伸了你的双手；GameFrameX 延伸的是你的整个团队——服务器是你运维能力的延伸，后台是你运营能力的延伸，CI 是你发布节奏的延伸。一个人加上 GameFrameX，就拥有过去一个团队的火力。

独立开发不该是孤军奋战：框架是武器，文档是地图，社区是同行的族人。从第一个原型到千万玩家，每一步都有同类同行。

### 功能特性

- **一份代码，四个引擎**：Unity、Cocos Creator、LayaBox、Godot 全支持，业务逻辑与引擎解耦。换引擎不等于重写游戏，同一个梦想在每个目标平台落地。
- **多进程服务器，从原型扛到上线**：网关、逻辑、数据各司其职，玩家多了就横向扩容。Docker 自动构建部署，环境一致——不再有「我本地是好的」。
- **发布只需一个 tag**：Codeup、CNB、GitHub Actions 三选一，接入团队既有的托管习惯。推 `tag` 即构建即部署，发布从一场仪式变成一次日常提交。
- **数据栈开箱即用**：MongoDB 存游戏数据，扛得住高并发读写；PostgreSQL 管后台，稳固可靠；LuBan 处理配置表，自动生成、保准确；Protobuf 定协议，客户端与服务器共用一套消息定义。
- **一体化后台，看得见你的玩家**：客户端管理、运维管理、数据管理、游戏运营。谁在玩、玩什么、卡在哪——上线之后，数据不再是黑盒。

## 快速开始

### 安装

三步跑起来：

1. 打开[快速开始指南](https://gameframex.doc.alianblank.com)
2. 按步骤把 GameFrameX 接入你的项目
3. 推第一个 `tag`，看 CI 把它变成一个可运行的服

从这一刻起，你面对的不是一堆零件，而是一条已经接好的流水线。

## 使用示例

**单人独立开发者**——一个人身兼程序、策划、运维：早上在 Unity 里调玩法，中午用 LuBan 拉一张配置表，下午推一个 `tag` 触发 CI 构建与部署，晚上在一体化后台看玩家数据。这就是 GameFrameX 为独立开发者准备的日常。

**小团队协作**——客户端与服务器共享同一套 Protobuf 协议与同一个数据语境；管理员与开发者的权限边界清晰；Codeup、CNB、GitHub Actions 三选一，接入团队既有的代码托管习惯，零迁移成本。

更多示例与教程请见[在线文档](https://gameframex.doc.alianblank.com)。

## 依赖

- **MongoDB** — 游戏数据库：高性能、灵活的数据存储方案，确保大规模和复杂数据的快速读写能力，增强游戏的扩展性和稳定性
- **PostgreSQL** — 后台管理数据库：提供稳固可靠的后端管理系统；与 MongoDB 相互配合，实现数据解决方案上多样性和功能性的平衡，满足不同场景下的业务需要
- **LuBan** — 数据表工具：自动化并优化数据表的处理流程，极大提高开发效率，并保证数据的准确性和一致性
- **Protobuf** — 网络通信协议：高效的二进制序列化方案，用于客户端与服务器、服务器进程之间的消息通信
- **Docker** — 自动化构建与部署，确保在不同环境下软件以同样的方式运行

## 文档与资源

`所有站点内容一致，不存在内容不一致的情况`

- 文档地址：https://gameframex.doc.alianblank.com
- 备用地址：https://gameframex-docs.pages.dev
- 备用地址：https://gameframex.doc.cloudflare.alianblank.com
- 备用地址：https://gameframex.doc.vercel.alianblank.com

## 社区与支持

![QQ](https://img.shields.io/badge/QQ-467608841%2F233840761-EB1923?style=for-the-badge&logo=qq&logoColor=white)
[![Bilibili](https://img.shields.io/badge/Bilibili-00A1D6?style=for-the-badge&logo=bilibili&logoColor=white)](https://www.bilibili.com/video/BV1yrpeepEn7)
[![Gitee](https://img.shields.io/badge/Gitee-C71D23?style=for-the-badge&logo=gitee&logoColor=white)](https://gitee.com/GameFrameX/gameframex)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GameFrameX/gameframex)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/VDWUjWMDw9)
[<img src="https://cdn.jsdelivr.net/npm/devicon@2/icons/linkedin/linkedin-original.svg" height="28" alt="LinkedIn" />](https://www.linkedin.com/in/alianblank)
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/r/GameFrameX/)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/alian_blank)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UCD9QhSFJ5xZkn5NTSV-DVAw)
[![Bluesky](https://img.shields.io/badge/Bluesky-0285FF?style=for-the-badge&logo=bluesky&logoColor=white)](https://bsky.app/profile/alianblank.bsky.social)

## 更新日志

最新动态请查看[在线文档](https://gameframex.doc.alianblank.com)。

## 免责声明

所有插件均来自互联网，请各位使用时自行付费。如果以上插件涉及侵权，请发 email 或提交 issue，本人将移除，谢谢。

该项目不得用于当地法律不允许的使用范围。如果使用，本人或本组织将不承认和承担任何的法律责任和条款约束。

技术本无罪，错的是滥用技术的人

## 开源协议

详见 [LICENSE.md](../LICENSE.md) 文件。

<!--
EN: See [LICENSE.md](../LICENSE.md) for license information.
zh-CN: 详见 [LICENSE.md](../LICENSE.md) 文件。
zh-TW: 詳見 [LICENSE.md](../LICENSE.md) 檔案。
ja: 詳しくは [LICENSE.md](../LICENSE.md) をご参照ください。
ko: 자세한 내용은 [LICENSE.md](../LICENSE.md) 파일을 참조하세요.
-->
