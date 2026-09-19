<div align="center">

<img src="https://download.alianblank.com/gameframex/gameframex_logo_320.png" alt="Game Frame X Logo" width="160" />

# GameFrameX

[![License](https://img.shields.io/badge/license-blue.svg)](../LICENSE.md)
[![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://gameframex.doc.alianblank.com)

[![Discord](https://img.shields.io/badge/-5865F2?logo=discord&logoColor=white)](https://discord.gg/VDWUjWMDw9)
[![GitHub](https://img.shields.io/badge/-181717?logo=github&logoColor=white)](https://github.com/GameFrameX/gameframex)
[![Bilibili](https://img.shields.io/badge/-00A1D6?logo=bilibili&logoColor=white)](https://www.bilibili.com/video/BV1yrpeepEn7)
[![Gitee](https://img.shields.io/badge/-C71D23?logo=gitee&logoColor=white)](https://gitee.com/GameFrameX/gameframex)

All-in-One Solution for Indie Game Development · Empowering Indie Developers' Dreams

<br />

[Documentation](https://gameframex.doc.alianblank.com) · [Quick Start](#quick-start) · QQ Group: 467608841 / 233840761

<br />

**English** | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | [한국어](README.ko.md)

</div>

## Project Overview

If you know C#, you can build an online game on your own. The hard part was never the gameplay — it's everything around it: writing the server, picking databases, wiring the config-table pipeline, setting up release CI, and finding a back office to watch player data after launch. GameFrameX hands you all of it at once: a multi-engine client, a multi-process server, a unified back office, and CI that works out of the box — one language, C#, across client and server, one set of Protobuf contracts. You focus on the gameplay; the framework has the rest assembled.

And you don't have to swallow it all in one bite. Start with the client alone and prototype your gameplay in the engine you already know; when you need multiplayer, add a C# server — the same language as your client, the same Protobuf contracts; when it's time to ship, the databases, back office, Docker, and CI are ready and waiting. The framework grows with your game, from the first prototype to millions of players, with no mid-journey stack swap.

Indie development should not be a lone battle: the framework is your weapon, the documentation your map, and the community your fellow travelers. One person plus GameFrameX equals the firepower that used to take a full team.

### Features

- **One codebase, four engines**: Unity, Cocos Creator, LayaBox, and Godot, with business logic decoupled from the engine. Switching engines does not mean rewriting your game — one dream lands on every target platform.
- **A multi-process server that scales from prototype to production**: gateway, logic, and data each play their part; add capacity when the players come. Docker-based build and deploy keeps every environment identical — no more "but it worked on my machine."
- **Shipping is one tag away**: Codeup, CNB, GitHub Actions, and beyond — mainstream pipelines work out of the box, and the one your team already runs plugs in just as well. Push a `tag` and the build and deployment take care of themselves; a release stops being a ritual and becomes an everyday commit.
- **A data stack that works out of the box**: MongoDB for game data, built for high-concurrency reads and writes; PostgreSQL for the back office, solid and reliable; LuBan for config tables, auto-generated and guaranteed accurate; Protobuf for the protocol, one set of message definitions shared by client and server.
- **A unified back office that shows you your players**: client management, ops management, data management, and game operations. Who is playing, what they play, where they get stuck — after launch, data is no longer a black box.

## Quick Start

### Installation

Get a game server running in three minutes — the full walkthrough is in the [Quick Start guide](https://gameframex.doc.alianblank.com).

## Usage Examples

**The solo indie developer** — one person wearing the hats of programmer, designer, and ops. Tune gameplay in Unity in the morning, pull a config table with LuBan at noon, push a `tag` in the afternoon to trigger a CI build and deploy, and watch player data on the unified back office in the evening. That is the daily routine GameFrameX prepares for indie developers.

**The small team** — client and server share the same Protobuf contracts and the same data context; permission boundaries between admins and developers stay clear; Codeup, CNB, GitHub Actions, and beyond — whatever CI the team already runs plugs right in, with zero migration cost.

**Games already live** — proof the framework holds up in real production:

- **Animal Garden (どうぶつの花屋)** — Simulation · App Store (JP) / Google Play (KR)
- **Late-Night BBQ (深夜的烧烤店)** — Idle Simulation · TapTap / App Store / Google Play
- **Endless Loop (连续黑白)** — Strategy · live in production
- **Dimensional Defense (异次元防线)** — Tower Defense · Google Play

More examples and tutorials are available in the [online documentation](https://gameframex.doc.alianblank.com).

## Dependencies

Nothing on this list you install and wire up by hand — the databases come up with a single `docker compose up`, and the LuBan and Protobuf toolchains are built into the framework's workflow:

- **MongoDB** — the game database: a high-performance, flexible storage solution that ensures fast reads and writes for large-scale and complex data, enhancing scalability and stability
- **PostgreSQL** — the back-office database: a solid and reliable admin system; combined with MongoDB, it balances diversity and functionality to meet different business scenarios
- **LuBan** — the data table tool: automates and optimizes the table processing pipeline, greatly improving development efficiency while guaranteeing data accuracy and consistency
- **Protobuf** — the network messaging layer: efficient binary serialization for client-server and inter-process communication
- **Docker** — automated build and deployment, ensuring the software runs the same way in every environment

## Documentation & Resources

`All sites serve identical content`

- Docs: https://gameframex.doc.alianblank.com
- Mirror: https://gameframex-docs.pages.dev
- Mirror: https://gameframex.doc.cloudflare.alianblank.com
- Mirror: https://gameframex.doc.vercel.alianblank.com

## Community & Support

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/GameFrameX/gameframex)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/VDWUjWMDw9)
[<img src="https://cdn.jsdelivr.net/npm/devicon@2/icons/linkedin/linkedin-original.svg" height="28" alt="LinkedIn" />](https://www.linkedin.com/in/alianblank)
[![Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/r/GameFrameX/)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/alian_blank)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://www.youtube.com/channel/UCD9QhSFJ5xZkn5NTSV-DVAw)
[![Bluesky](https://img.shields.io/badge/Bluesky-0285FF?style=for-the-badge&logo=bluesky&logoColor=white)](https://bsky.app/profile/alianblank.bsky.social)
[![Bilibili](https://img.shields.io/badge/Bilibili-00A1D6?style=for-the-badge&logo=bilibili&logoColor=white)](https://www.bilibili.com/video/BV1yrpeepEn7)
[![Gitee](https://img.shields.io/badge/Gitee-C71D23?style=for-the-badge&logo=gitee&logoColor=white)](https://gitee.com/GameFrameX/gameframex)
![QQ](https://img.shields.io/badge/QQ-467608841%2F233840761-EB1923?style=for-the-badge&logo=qq&logoColor=white)

## Changelog

See the [online documentation](https://gameframex.doc.alianblank.com) for the latest updates.

## Disclaimer

All plugins come from the internet. Please pay for them yourself where required. If any plugin involves copyright infringement, please send an email or open an issue, and it will be removed. Thank you.

This project must not be used for purposes prohibited by local laws. If used, neither the owner nor this organization will recognize or assume any legal liability or be bound by any such terms.

Technology itself is innocent; those who abuse it are at fault.

## License

See [LICENSE.md](../LICENSE.md) for license information.

<!--
EN: See [LICENSE.md](../LICENSE.md) for license information.
zh-CN: 详见 [LICENSE.md](../LICENSE.md) 文件。
zh-TW: 詳見 [LICENSE.md](../LICENSE.md) 檔案。
ja: 詳しくは [LICENSE.md](../LICENSE.md) をご参照ください。
ko: 자세한 내용은 [LICENSE.md](../LICENSE.md) 파일을 참조하세요.
-->
