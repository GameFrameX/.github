<div align="center">

<img src="https://download.alianblank.com/gameframex/gameframex_logo_320.png" alt="Game Frame X Logo" width="160" />

# GameFrameX

[![License](https://img.shields.io/badge/license-blue.svg)](../LICENSE.md)
[![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://gameframex.doc.alianblank.com)

[![Discord](https://img.shields.io/badge/-5865F2?logo=discord&logoColor=white)](https://discord.gg/VDWUjWMDw9)
[![GitHub](https://img.shields.io/badge/-181717?logo=github&logoColor=white)](https://github.com/GameFrameX/gameframex)
[![Bilibili](https://img.shields.io/badge/-00A1D6?logo=bilibili&logoColor=white)](https://www.bilibili.com/video/BV1yrpeepEn7)
[![Gitee](https://img.shields.io/badge/-C71D23?logo=gitee&logoColor=white)](https://gitee.com/GameFrameX/gameframex)

獨立遊戲前後端一體化解決方案 · 獨立遊戲開發者的圓夢大使

<br />

[文檔](https://gameframex.doc.alianblank.com) · [快速開始](#快速開始) · QQ群: 467608841 / 233840761

<br />

[English](README.md) | [简体中文](README.zh-CN.md) | **繁體中文** | [日本語](README.ja.md) | [한국어](README.ko.md)

</div>

## 項目簡介

會 C#，就能一個人做完一款連網遊戲。難的從來不是玩法，而是玩法之外的一切：寫伺服器、選資料庫、搭配置表流程、配發布 CI——上線之後，還得有後台看玩家數據。GameFrameX 把這些一次性組裝好：多引擎客戶端、多進程伺服器、一體化後台、開箱即用的 CI——前後端同一門 C#、同一套 Protobuf 協定。你只管專注玩法，剩下的框架已經備好。

不必一口吞下全家桶。先只用客戶端，在你熟悉的引擎裡把玩法原型跑起來；需要連網了，加一個 C# 伺服器——與客戶端同一門語言、同一套 Protobuf 協定；要上線了，資料庫、後台、Docker、CI 隨時在位。框架隨遊戲一起長大，從第一個原型到千萬玩家，不用中途換棧。

獨立開發不該是孤軍奮戰：框架是武器，文檔是地圖，社群是同行的族人。一個人加上 GameFrameX，就擁有過去一個團隊的火力。

### 功能特性

- **一份程式碼，四個引擎**：Unity、Cocos Creator、LayaBox、Godot 全支援，業務邏輯與引擎解耦。換引擎不等於重寫遊戲，同一個夢想在每個目標平台落地。
- **多進程伺服器，從原型扛到上線**：閘道、邏輯、數據各司其職，玩家多了就橫向擴容。Docker 自動構建部署，環境一致——不再有「我本地是好的」。
- **發布只需一個 tag**：Codeup、CNB、GitHub Actions 等主流流水線平台開箱即用，其他 CI 方案同樣接得進來。推 `tag` 即構建即部署，發布從一場儀式變成一次日常提交。
- **數據棧開箱即用**：MongoDB 存遊戲數據，扛得住高併發讀寫；PostgreSQL 管後台，穩固可靠；LuBan 處理配置表，自動生成、保準確；Protobuf 定協定，客戶端與伺服器共用一套訊息定義。
- **一體化後台，看得見你的玩家**：客戶端管理、維運管理、數據管理、遊戲營運。誰在玩、玩什麼、卡在哪——上線之後，數據不再是黑盒。

## 快速開始

### 安裝

三分鐘把伺服器跑起來——完整步驟見[快速開始指南](https://gameframex.doc.alianblank.com)。

## 使用範例

**單人獨立開發者**——一個人身兼程式、策劃、維運：早上在 Unity 裡調玩法，中午用 LuBan 拉一張配置表，下午推一個 `tag` 觸發 CI 構建與部署，晚上在一體化後台看玩家數據。這就是 GameFrameX 為獨立開發者準備的日常。

**小團隊協作**——客戶端與伺服器共享同一套 Protobuf 協議與同一個數據語境；管理員與開發者的權限邊界清晰；Codeup、CNB、GitHub Actions 等主流流水線開箱即用，團隊既有的其他 CI 方案同樣接得進來，零遷移成本。

**已上線的遊戲**——框架扛過真實營運的證明：

- **Animal Garden（どうぶつの花屋）** — 模擬經營 · 日本 App Store / 韓國 Google Play
- **深夜的燒烤店** — 放置模擬 · TapTap / App Store / Google Play
- **連續黑白** — 策略 · 已上線
- **異次元防線** — 塔防 · Google Play

更多範例與教程請見[線上文檔](https://gameframex.doc.alianblank.com)。

## 依賴

這份清單不需要逐個安裝配置——資料庫由 Docker Compose 一鍵拉起，LuBan 與 Protobuf 工具鏈已內置在框架的開發流程裡：

- **MongoDB** — 遊戲資料庫：高效能、靈活的資料儲存方案，確保大規模和複雜資料的快速讀寫能力，增強遊戲的擴展性和穩定性
- **PostgreSQL** — 後台管理資料庫：提供穩固可靠的後端管理系統；與 MongoDB 相互配合，實現資料解決方案上多樣性和功能性的平衡，滿足不同場景下的業務需要
- **LuBan** — 數據表工具：自動化並最佳化數據表的處理流程，極大提高開發效率，並保證數據的準確性和一致性
- **Protobuf** — 網路通訊協定：高效的二進位序列化方案，用於客戶端與伺服器、伺服器進程之間的訊息通訊
- **Docker** — 自動化構建與部署，確保在不同環境下軟體以同樣的方式運行

## 文檔與資源

`所有站點內容一致，不存在內容不一致的情況`

- 文檔地址：https://gameframex.doc.alianblank.com
- 備用地址：https://gameframex-docs.pages.dev
- 備用地址：https://gameframex.doc.cloudflare.alianblank.com
- 備用地址：https://gameframex.doc.vercel.alianblank.com

## 社區與支援

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

## 更新日誌

最新動態請查看[線上文檔](https://gameframex.doc.alianblank.com)。

## 免責聲明

所有插件均來自互聯網，請各位使用時自行付費。如果以上插件涉及侵權，請發 email 或提交 issue，本人將移除，謝謝。

該項目不得用於當地法律不允許的使用範圍。如果使用，本人或本組織將不承認和承擔任何的法律責任和條款約束。

技術本無罪，錯的是濫用技術的人

## 開源協議

詳見 [LICENSE.md](../LICENSE.md) 檔案。

<!--
EN: See [LICENSE.md](../LICENSE.md) for license information.
zh-CN: 详见 [LICENSE.md](../LICENSE.md) 文件。
zh-TW: 詳見 [LICENSE.md](../LICENSE.md) 檔案。
ja: 詳しくは [LICENSE.md](../LICENSE.md) をご参照ください。
ko: 자세한 내용은 [LICENSE.md](../LICENSE.md) 파일을 참조하세요.
-->
