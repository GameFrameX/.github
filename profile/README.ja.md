<div align="center">

<img src="https://download.alianblank.com/gameframex/gameframex_logo_320.png" alt="Game Frame X Logo" width="160" />

# GameFrameX

[![License](https://img.shields.io/badge/license-blue.svg)](../LICENSE.md)
[![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://gameframex.doc.alianblank.com)

[![Discord](https://img.shields.io/badge/-5865F2?logo=discord&logoColor=white)](https://discord.gg/VDWUjWMDw9)
[![GitHub](https://img.shields.io/badge/-181717?logo=github&logoColor=white)](https://github.com/GameFrameX/gameframex)
[![Bilibili](https://img.shields.io/badge/-00A1D6?logo=bilibili&logoColor=white)](https://www.bilibili.com/video/BV1yrpeepEn7)
[![Gitee](https://img.shields.io/badge/-C71D23?logo=gitee&logoColor=white)](https://gitee.com/GameFrameX/gameframex)

インディゲーム開発者向けオールインワンソリューション · インディ開発者の夢を支援

<br />

[ドキュメント](https://gameframex.doc.alianblank.com) · [クイックスタート](#クイックスタート) · QQグループ: 467608841 / 233840761

<br />

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | **日本語** | [한국어](README.ko.md)

</div>

## プロジェクト概要

C# が書ければ、オンラインゲームを一人で完成させられます。難しさはゲームプレイそのものではなく、その周りにあります：サーバーの実装、データベースの選定、コンフィグテーブルのパイプライン、リリース CI——ローンチ後には、プレイヤーデータを見るための管理画面まで。GameFrameX はこれらを一度にすべて提供します：マルチエンジンのクライアント、マルチプロセスのサーバー、統合管理画面、すぐに使える CI——クライアントとサーバーは同じ C#、同じ Protobuf プロトコル。あなたはゲームプレイに集中してください——残りは、フレームワークがすでに組み上げてあります。

しかも、すべてを一度に飲み込む必要はありません。まずはクライアントだけで、慣れたエンジンでゲームプレイのプロトタイプを走らせる。マルチプレイが必要になったら C# サーバーを追加——クライアントと同じ言語、同じ Protobuf プロトコル。リリースの段階では、データベースも管理画面も Docker も CI も、もうそこにあります。フレームワークはゲームと一緒に成長し、最初のプロトタイプから数百万のプレイヤーまで、途中でスタックを乗り換える必要はありません。

インディ開発は、一人で戦うものであるべきではありません。フレームワークは武器、ドキュメントは地図、コミュニティは同行する仲間。一人の開発者に GameFrameX が加われば、かつてチーム全体で持っていた火力になります。

### 機能概要

- **ひとつのコードベースで、4つのエンジン**：Unity、Cocos Creator、LayaBox、Godot に対応。ビジネスロジックはエンジンから分離され、エンジンを乗り換えてもゲームを作り直すことにはなりません。同じ夢が、すべてのターゲットプラットフォームで根を下ろします。
- **プロトタイプから本番まで耐えるマルチプロセスサーバー**：ゲートウェイ、ロジック、データがそれぞれ役割を担い、プレイヤーが増えれば横にスケール。Docker によるビルドとデプロイで環境はいつも同一——「ローカルでは動いていた」はもう言わなくて大丈夫です。
- **リリースは tag ひとつ**：Codeup、CNB、GitHub Actions など主要なパイプラインはすぐ使え、チームが使っているほかの CI サービスとも組み合わせられます。`tag` をプッシュすればビルドもデプロイも自分で世話をしてくれます。リリースは儀式ではなく、いつものコミットになります。
- **箱から出してすぐ使えるデータスタック**：ゲームデータは MongoDB（高並行な読み書きに耐える設計）、管理画面は PostgreSQL（堅牢で信頼できる）、コンフィグテーブルは LuBan（自動生成・正確性保証）、プロトコルは Protobuf（クライアントとサーバーが同じメッセージ定義を共有）。
- **プレイヤーが見える統合管理画面**：クライアント管理・運用管理・データ管理・ゲーム運営。誰が遊んでいて、何を遊んでいて、どこで詰まっているのか——ローンチ後、データはもう黒箱ではありません。

## クイックスタート

### インストール

3 分でゲームサーバーを起動できます——完全な手順は[クイックスタートガイド](https://gameframex.doc.alianblank.com)にあります。

## 使用例

**ソロのインディ開発者**——プログラマー、プランナー、運用を一人で兼ねる。朝は Unity でゲームプレイを調整し、昼は LuBan でコンフィグテーブルを作り、午後は `tag` をプッシュして CI のビルドとデプロイを起こし、夜は統合管理画面でプレイヤーデータを見る。それが GameFrameX がインディ開発者のために用意した日常です。

**小規模チーム**——クライアントとサーバーは同じ Protobuf コントラクトと同じデータ文脈を共有し、管理者と開発者の権限の境界は明確。Codeup、CNB、GitHub Actions など主要なパイプラインはすぐ使え、チームが使っているほかの CI サービスとも組み合わせられます。移行コストはゼロです。

**すでにリリースされているゲーム**——フレームワークが実運用を耐え抜いた証：

- **Animal Garden（どうぶつの花屋）** — 経営シミュレーション · 日本 App Store / 韓国 Google Play
- **深夜的烧烤店（Late-Night BBQ）** — 放置系シミュレーション · TapTap / App Store / Google Play
- **连续黑白（Endless Loop）** — ストラテジー · リリース済み
- **异次元防线（Dimensional Defense）** — タワーディフェンス · Google Play

その他の使用例とチュートリアルは[オンラインドキュメント](https://gameframex.doc.alianblank.com)で公開しています。

## 依存関係

このリストを一つずつインストール・設定する必要はありません——データベースは `docker compose up` 1 回で立ち上がり、LuBan と Protobuf のツールチェーンはフレームワークのワークフローに組み込まれています：

- **MongoDB** — ゲームデータベース：大規模・複雑なデータの高速な読み書きを保証する、高性能で柔軟なストレージソリューション
- **PostgreSQL** — 管理用データベース：堅牢で信頼性の高い管理システム。MongoDB との組み合わせで、多様なビジネスシーンのニーズに対応
- **LuBan** — データテーブルツール：テーブル処理のパイプラインを自動化・最適化し、正確性と一貫性を保証
- **Protobuf** — ネットワーク通信プロトコル：クライアントとサーバー、サーバープロセス間のメッセージ通信に使用する高速なバイナリシリアライズ方式
- **Docker** — 自動ビルドとデプロイにより、どの環境でも同じように動作

## ドキュメントとリソース

`すべてのサイトの内容は同一です`

- ドキュメント: https://gameframex.doc.alianblank.com
- ミラー: https://gameframex-docs.pages.dev
- ミラー: https://gameframex.doc.cloudflare.alianblank.com
- ミラー: https://gameframex.doc.vercel.alianblank.com

## コミュニティとサポート

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

## 変更履歴

最新の更新は[オンラインドキュメント](https://gameframex.doc.alianblank.com)をご覧ください。

## 免責事項

すべてのプラグインはインターネット上のものです。必要な場合は各自で購入してください。プラグインが権利を侵害している場合は、メールまたは issue をお送りいただければ削除します。

本プロジェクトは、現地の法律で許可されていない用途には使用できません。使用された場合、本人および本組織は一切の法的責任および契約上の義務を負いません。

技術そのものに罪はなく、それを濫用する人に問題があります

## ライセンス

詳しくは [LICENSE.md](../LICENSE.md) をご参照ください。

<!--
EN: See [LICENSE.md](../LICENSE.md) for license information.
zh-CN: 详见 [LICENSE.md](../LICENSE.md) 文件。
zh-TW: 詳見 [LICENSE.md](../LICENSE.md) 檔案。
ja: 詳しくは [LICENSE.md](../LICENSE.md) をご参照ください。
ko: 자세한 내용은 [LICENSE.md](../LICENSE.md) 파일을 참조하세요.
-->
