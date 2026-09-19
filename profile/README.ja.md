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

開発体験を本当に変えるのは、機能のスペック表ではなく、フレームワーク全体が組織される方式です。道具の構造は、やがてあなたの仕事のリズムになります。

GameFrameX は、クライアント、サーバー、データ、運用をひとつの統合構造に収めます。導入初日から、それはあなたの開発リズムと知覚のあり方そのものを組み替えます。ツールチェーンを接着して回る作業から離れ、完全な開発エコシステムを運営する——構想からリリース、リリースから長期運営まで、すべてが同じ文脈の中で流れていきます。

ゲームエンジンがあなたの両手を延長し、世界を描く筆を与えるなら、GameFrameX が延長するのはチーム全体です。マルチプロセスサーバーは運用力の延長、統合管理画面は運営力の延長、3 プラットフォーム CI はリリース間隔の延長。一人の開発者に GameFrameX が加われば、かつてチーム全体で持っていた火力になります。

インディ開発は、一人で戦うものであるべきではありません。GameFrameX があなたに返したいのは「部族」です。フレームワークは武器、ドキュメントは地図、コミュニティは同行する仲間。最初のプロトタイプから数百万のプレイヤーまで、一歩ごとに仲間がいます。

### 機能概要

- **ひとつのコードベースで、主要プラットフォーム全覆盖**：Unity、Cocos Creator、LayaBox、Godot に対応。ビジネスロジックはエンジン選択から分離され、アイデアが単一プラットフォームに閉じ込められることはなく、同じ夢がすべてのターゲットプラットフォームで根を下ろします。
- **マルチプロセスサーバー構成 — 規模の天井を外す**：ゲートウェイ、ロジック、データがそれぞれ役割を担い、水平スケーリングも余裕をもこなします。Docker による自動ビルド・デプロイで、パッケージングと配布は効率化・標準化され、どの環境でも同じように動作します。
- **3 プラットフォーム CI/CD：Codeup、CNB、GitHub Actions**：`tag` をプッシュすればビルドが走ります。リリースは慎重な儀式から、いつもの呼吸へ——変更管理は連続し、デプロイは自動、手作業は最小限に。
- **データスタックがそれぞれの場所に**：MongoDB はゲームデータの高並行な読み書きを支え、PostgreSQL は堅牢な管理画面の土台となり、LuBan はテーブル処理を自動化して正確さを保証し、Protobuf の高速バイナリシリアライズがクライアントとサーバー、プロセスとプロセスの対話をつなぎます。
- **統合管理画面 — 運営力の延長**：クライアント管理・運用管理・データ管理・ゲームデータ運営。ライブゲームの監視・最適化・更新はかつてないほど簡単になり、リソースは効率よく配分され、開発サイクルは短く、運用コストは低く、プレイヤー体験はより良くなります。

## クイックスタート

### インストール

オンラインドキュメントの[クイックスタートガイド](https://gameframex.doc.alianblank.com)に従って、GameFrameX をプロジェクトに導入してください。その瞬間から、あなたの前にあるのは部品の山ではなく、組み立て済みの開発環境です。

## 使用例

**ソロのインディ開発者**——プログラマー、プランナー、運用を一人で兼ねる。朝は Unity でゲームプレイを調整し、昼は LuBan でコンフィグテーブルを作り、午後は `tag` をプッシュして CI のビルドとデプロイを起こし、夜は統合管理画面でプレイヤーデータを見る。それが GameFrameX がインディ開発者のために用意した日常です。

**小規模チーム**——クライアントとサーバーは同じ Protobuf コントラクトと同じデータ文脈を共有し、管理者と開発者の権限の境界は明確。Codeup、CNB、GitHub Actions の 3 択から、チームの既存ホスティング習慣に合うものを選べばよく、移行コストはゼロです。

その他の使用例とチュートリアルは[オンラインドキュメント](https://gameframex.doc.alianblank.com)で公開しています。

## 依存関係

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
