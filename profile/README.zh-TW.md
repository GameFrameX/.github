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

真正改變開發體驗的，從來不是某個功能點的參數表，而是整個框架被組織的方式。工具的結構，會慢慢變成你工作的節奏。

GameFrameX 把客戶端、伺服器、數據與營運裝進同一個一體化結構。從接入的第一天起，它重塑的就是你的開發節奏與感知方式：你不再忙於拼湊和黏合工具鏈，而是在經營一個完整的開發生態——從構想到上線，從上線到長線營運，一切都在同一個語境裡流動。

遊戲引擎延伸了你的雙手，讓你擁有創造世界的筆觸；GameFrameX 延伸的是你的整個團隊——多進程伺服器是你維運能力的延伸，一體化後台是你營運能力的延伸，三平台 CI 流水線是你發布節奏的延伸。一個人加上 GameFrameX，就擁有過去一個團隊的火力。

獨立開發不該是一場孤軍奮戰。GameFrameX 想還給你的，是一個部落：框架是武器，文檔是地圖，社群是同行的族人。從第一個原型到千萬玩家，每一步都有同類同行。

### 功能特性

- **一份程式碼，覆蓋所有主流平台**：Unity、Cocos Creator、LayaBox、Godot 全支援。業務邏輯與引擎選型解耦，創意不被單一平台鎖死，同一個夢想在每個目標平台落地生根。
- **多進程伺服器架構，規模不再是天花板**：閘道、邏輯、數據各司其職，橫向擴展從容不迫。配套 Docker 自動化構建與部署，打包、分發高效且標準化，應用在不同環境下以同樣的方式運行。
- **三平台 CI/CD：Codeup、CNB、GitHub Actions**：`tag` 一推，構建即走。發布從一場小心翼翼的儀式，變成一次隨手的呼吸——變更連貫管理、部署全自動，人工干預降到最低。
- **數據棧各就其位**：MongoDB 承載遊戲數據的高併發讀寫；PostgreSQL 支撐穩固的後台管理；LuBan 讓數據表處理自動化、保準確；Protobuf 以高效二進位序列化，打通客戶端與伺服器、進程與進程之間的每一次對話。
- **一體化後台，營運能力的延伸**：客戶端管理、維運管理、數據管理、遊戲數據營運——監控、最佳化與更新前所未有地簡單。資源高效分配，開發週期更短，營運成本更低，玩家體驗更好。

## 快速開始

### 安裝

跟隨線上文檔中的[快速開始指南](https://gameframex.doc.alianblank.com)，把 GameFrameX 接入你的專案。從這一刻起，你面對的就不再是一堆零件，而是一個組裝完畢的開發環境。

## 使用範例

**單人獨立開發者**——一個人身兼程式、策劃、維運：早上在 Unity 裡調玩法，中午用 LuBan 拉一張配置表，下午推一個 `tag` 觸發 CI 構建與部署，晚上在一體化後台看玩家數據。這就是 GameFrameX 為獨立開發者準備的日常。

**小團隊協作**——客戶端與伺服器共享同一套 Protobuf 協議與同一個數據語境；管理員與開發者的權限邊界清晰；Codeup、CNB、GitHub Actions 三選一，接入團隊既有的程式碼託管習慣，零遷移成本。

更多範例與教程請見[線上文檔](https://gameframex.doc.alianblank.com)。

## 依賴

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
