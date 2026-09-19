<div align="center">

<img src="https://download.alianblank.com/gameframex/gameframex_logo_320.png" alt="Game Frame X Logo" width="160" />

# GameFrameX

[![License](https://img.shields.io/badge/license-blue.svg)](../LICENSE.md)
[![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://gameframex.doc.alianblank.com)

[![Discord](https://img.shields.io/badge/-5865F2?logo=discord&logoColor=white)](https://discord.gg/VDWUjWMDw9)
[![GitHub](https://img.shields.io/badge/-181717?logo=github&logoColor=white)](https://github.com/GameFrameX/gameframex)
[![Bilibili](https://img.shields.io/badge/-00A1D6?logo=bilibili&logoColor=white)](https://www.bilibili.com/video/BV1yrpeepEn7)
[![Gitee](https://img.shields.io/badge/-C71D23?logo=gitee&logoColor=white)](https://gitee.com/GameFrameX/gameframex)

인디 게임 개발자를 위한 올인원 솔루션 · 인디 개발자의 꿈을 실현

<br />

[문서](https://gameframex.doc.alianblank.com) · [빠른 시작](#빠른-시작) · QQ 그룹: 467608841 / 233840761

<br />

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | **한국어**

</div>

## 프로젝트 개요

C#를 안다면 온라인 게임을 혼자서 완성할 수 있습니다. 어려운 것은 게임플레이가 아니라 그 주변의 모든 것입니다: 서버 구현, 데이터베이스 선정, 설정 테이블 파이프라인 구축, 릴리스 CI — 출시 후에는 플레이어 데이터를 볼 백오피스까지. GameFrameX는 이 모든 것을 한 번에 제공합니다: 멀티 엔진 클라이언트, 멀티 프로세스 서버, 통합 백오피스, 바로 쓸 수 있는 CI — 클라이언트와 서버는 같은 C#, 같은 Protobuf 프로토콜. 당신은 게임플레이에만 집중하세요 — 나머지는 프레임워크가 이미 조립해 두었습니다.

한 번에 전부 받아들일 필요도 없습니다. 우선 클라이언트만으로, 익숙한 엔진에서 게임플레이 프로토타입을 만드세요. 멀티플레이가 필요해지면 C# 서버를 추가하면 됩니다 — 클라이언트와 같은 언어, 같은 Protobuf 프로토콜. 출시가 다가오면 데이터베이스, 백오피스, Docker, CI가 이미 자리를 지키고 있습니다. 프레임워크는 게임과 함께 성장하여, 첫 프로토타입에서 수백만 플레이어까지 중간에 스택을 갈아탈 필요가 없습니다.

인디 개발은 혼자 싸우는 것이어서는 안 됩니다. 프레임워크는 무기이고, 문서는 지도이며, 커뮤니티는 함께 걷는 동족입니다. 한 사람에게 GameFrameX가 더해지면, 예전에 팀 전체가 가졌던 화력을 갖게 됩니다.

### 기능

- **하나의 코드베이스, 네 개의 엔진**: Unity, Cocos Creator, LayaBox, Godot 지원. 비즈니스 로직은 엔진과 분리되어 엔진을 바꾼다고 게임을 다시 만드는 것은 아닙니다. 같은 꿈이 모든 대상 플랫폼에 뿌리내립니다.
- **프로토타입부터 출시까지 버티는 멀티 프로세스 서버**: 게이트웨이, 로직, 데이터가 저마다 역할을 맡고, 플레이어가 늘면 수평으로 확장합니다. Docker 기반 빌드와 배포로 환경은 언제나 동일 — "제 로컬에서는 됐는데"는 이제 그만.
- **릴리스는 tag 하나로**: Codeup, CNB, GitHub Actions 등 주요 파이프라인은 물론, 팀이 이미 쓰고 있는 다른 CI도 그대로 연결됩니다. `tag`를 푸시하면 빌드와 배포가 알아서 돌아가고, 릴리스는 의식이 아니라 일상적인 커밋이 됩니다.
- **꺼내자마자 쓰는 데이터 스택**: 게임 데이터는 MongoDB(고병렬 읽기·쓰기 감당), 백오피스는 PostgreSQL(견고하고 안정적), 설정 테이블은 LuBan(자동 생성, 정확성 보장), 프로토콜은 Protobuf(클라이언트와 서버가 같은 메시지 정의를 공유).
- **플레이어가 보이는 통합 백오피스**: 클라이언트 관리, 운영 관리, 데이터 관리, 게임 운영. 누가 플레이하고, 무엇을 플레이하고, 어디서 막히는지 — 출시 후 데이터는 더 이상 블랙박스가 아닙니다.

## 빠른 시작

### 설치

3 분 만에 게임 서버를 실행할 수 있습니다 — 전체 단계는 [빠른 시작 가이드](https://gameframex.doc.alianblank.com)를 참고하세요.

## 사용 예시

**1인 인디 개발자** — 프로그래머, 기획자, 운영자를 한 사람이 겸합니다. 아침에는 Unity에서 게임플레이를 다듬고, 점심에는 LuBan으로 설정 테이블을 뽑고, 오후에는 `tag`를 푸시해 CI 빌드와 배포를 일으키고, 저녁에는 통합 백오피스에서 플레이어 데이터를 봅니다. 이것이 GameFrameX가 인디 개발자를 위해 준비한 일상입니다.

**소규모 팀** — 클라이언트와 서버는 같은 Protobuf 계약과 같은 데이터 맥락을 공유하고, 관리자와 개발자의 권한 경계는 명확합니다. Codeup, CNB, GitHub Actions 등 주요 파이프라인은 물론, 팀이 이미 쓰고 있는 다른 CI도 그대로 연결됩니다 — 마이그레이션 비용은 0입니다.

**이미 출시된 게임** — 프레임워크가 실제 운영을 견뎌낸 증거:

- **Animal Garden（どうぶつの花屋）** — 시뮬레이션 · 일본 App Store / 한국 Google Play
- **深夜的烧烤店（Late-Night BBQ）** — 방치형 시뮬레이션 · TapTap / App Store / Google Play
- **连续黑白（Endless Loop）** — 전략 · 출시됨
- **异次元防线（Dimensional Defense）** — 타워 디펜스 · Google Play

더 많은 예시와 튜토리얼은 [온라인 문서](https://gameframex.doc.alianblank.com)에서 확인할 수 있습니다.

## 의존성

이 목록을 하나씩 직접 설치·구성할 필요는 없습니다 — 데이터베이스는 `docker compose up` 한 번으로 뜨고, LuBan과 Protobuf 도구 체인은 프레임워크 워크플로에 내장되어 있습니다:

- **MongoDB** — 게임 데이터베이스: 대규모·복잡한 데이터의 빠른 읽기와 쓰기를 보장하는 고성능·유연한 스토리지 솔루션
- **PostgreSQL** — 관리용 데이터베이스: 견고하고 안정적인 관리 시스템 제공. MongoDB와 함께 다양한 비즈니스 시나리오의 요구를 충족
- **LuBan** — 데이터 테이블 도구: 테이블 처리 파이프라인을 자동화·최적화하여 정확성과 일관성 보장
- **Protobuf** — 네트워크 통신 프로토콜: 클라이언트와 서버, 서버 프로세스 간 메시지 통신에 사용되는 고속 바이너리 직렬화 방식
- **Docker** — 자동 빌드와 배포로 어떤 환경에서도 동일하게 동작

## 문서 및 자료

`모든 사이트의 내용은 동일합니다`

- 문서: https://gameframex.doc.alianblank.com
- 미러: https://gameframex-docs.pages.dev
- 미러: https://gameframex.doc.cloudflare.alianblank.com
- 미러: https://gameframex.doc.vercel.alianblank.com

## 커뮤니티 및 지원

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

## 변경 로그

최신 업데이트는 [온라인 문서](https://gameframex.doc.alianblank.com)를 참고하세요.

## 면책 조항

모든 플러그인은 인터넷에서 가져온 것입니다. 필요한 경우 각자 결제하여 사용하세요. 플러그인이 저작권을 침해하는 경우 이메일 또는 issue를 보내주시면 삭제하겠습니다.

본 프로젝트는 현지 법률에서 허용하지 않는 용도로 사용할 수 없습니다. 사용할 경우 본인 및 본 조직은 어떠한 법적 책임이나 약관의 구속도 인정하지 않습니다.

기술 자체는 죄가 없으며, 기술을 남용하는 사람이 잘못입니다

## 라이선스

자세한 내용은 [LICENSE.md](../LICENSE.md) 파일을 참조하세요.

<!--
EN: See [LICENSE.md](../LICENSE.md) for license information.
zh-CN: 详见 [LICENSE.md](../LICENSE.md) 文件。
zh-TW: 詳見 [LICENSE.md](../LICENSE.md) 檔案。
ja: 詳しくは [LICENSE.md](../LICENSE.md) をご参照ください。
ko: 자세한 내용은 [LICENSE.md](../LICENSE.md) 파일을 참조하세요.
-->
