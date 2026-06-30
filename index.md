# Privacy Policy / 隐私政策

**Last updated / 最后更新：2026-06-27**

---

## English

### 1. Introduction

N1 (the "App") is a Japanese reading and study application for JLPT N2-N1 learners,
developed and operated by an individual developer ("we", "us"). This Privacy Policy
explains what data we collect, how we use it, and your rights.

### 2. Data we do **not** collect

- **No user accounts.** The App does not require sign-up, email, phone number, or social-media login.
- **No personally identifiable information (PII).** We do not collect your name, email, location, contacts, IDFA, or any device identifier that can identify you.
- **No analytics SDKs.** No Firebase, Google Analytics, Sentry, Mixpanel, or comparable third-party telemetry.
- **No advertising.** No ads, no ad networks, no profiling.
- **No social features.** No sharing, no comments, no UGC visible to others.

### 3. Data we do collect / process

| Data | Purpose | Storage | Sent to server? |
|---|---|---|---|
| Japanese text you paste, URLs you import, words you tap | NLP analysis (tokenization, grammar annotation, translation, quiz generation) | Locally on your device (SQLite + AsyncStorage). Optionally sent to our backend for processing. | Yes — temporarily, for the duration of the request only |
| Reading progress, mastered/flagged words, quiz answers | Tracking your learning progress and powering the "memory star map" | Locally on your device only | **No** — never leaves your device |
| Invite code | Beta access control to prevent backend abuse | Locally on your device + sent as HTTP header to our backend on each API call | Yes — for authorization |

### 4. How server-side processing works

When you import an article, look up a word, request a translation, or generate a quiz,
your request is sent to our cloud server over HTTPS. The server processes the request
and returns the result. **We do not persist your content** in any database. Standard
hosting-platform request logs may briefly include the first ~50 characters of a request
body for debugging; these logs are ephemeral and automatically rotated.

### 5. Third parties involved in processing

To deliver core functionality the backend uses:

- A third-party Large Language Model service — for grammar annotation, translation, and quiz generation. Your text snippets are sent to that service for inference and are not retained.
- A third-party article-extraction service — for fetching the body content of URLs you submit.
- A cloud hosting provider — for hosting our backend.

We do not send your data to any third party for marketing or analytics purposes.

### 6. Data security

All client-server traffic uses HTTPS (TLS 1.2+). Your learning data
(articles, mastered words, progress) lives only on your device in the app sandbox;
uninstalling the App permanently erases it.

### 7. Children's privacy

The App is not directed to children under 13 and we do not knowingly collect any
data from children under 13.

### 8. Your rights

You can:
- **Delete all your data** by uninstalling the App.
- **Stop using the App at any time** with no obligation.

Because we do not collect identifiable data, there is no account to delete and no
data to export from our servers.

### 9. Changes to this policy

We may update this policy from time to time. The "Last updated" date at the top
will reflect any changes. Material changes will be surfaced in the App itself.

### 10. Contact

Questions about this policy or your data:

**Email: kyoi.cn@gmail.com**

---

## 中文

### 1. 简介

N1（以下简称「本应用」）是一款面向 JLPT N2-N1 学习者的日语阅读学习应用，
由个人开发者（「我们」）独立开发与运营。本隐私政策说明我们收集 / 处理哪些数据，
以及你的权利。

### 2. 我们**不**收集的数据

- **不需要账号。** 本应用不要求注册、不要求邮箱 / 手机号 / 社交登录。
- **不收集个人身份信息（PII）。** 我们不收集你的姓名、邮箱、地理位置、通讯录、IDFA 或任何可识别你身份的设备标识。
- **不接入数据分析 SDK。** 没有 Firebase / Google Analytics / Sentry / Mixpanel 等第三方埋点。
- **没有广告。** 不显示广告、不接入广告网络、不做用户画像。
- **没有社交功能。** 没有分享 / 评论 / 用户互见的 UGC。

### 3. 我们处理的数据

| 数据 | 用途 | 存储位置 | 是否发送到服务器 |
|---|---|---|---|
| 你粘贴的日文、导入的网址、点击查询的词汇 | 自然语言分析（分词、语法标注、翻译、出题）| 本地（设备 SQLite + AsyncStorage），按需发送服务器临时处理 | 是——仅在请求期间临时发送 |
| 阅读进度、已掌握 / 标记的词汇、测验答题记录 | 追踪学习进度、驱动「记忆星图」可视化 | **仅本地** | **否**——永远不离开你的设备 |
| 邀请码 | 内测期访问控制，防止后端被滥用 | 本地保存 + 每次 API 调用时通过 HTTP 头发给后端 | 是——用于授权 |

### 4. 服务端处理的机制

当你导入文章、查询词义、请求翻译或生成测验题时，请求通过 HTTPS 发送到我们的云端服务器。
服务器处理后返回结果。**我们不会把你的内容持久化到任何数据库**。托管平台的默认请求日志
可能会临时记录请求体的前 ~50 个字符用于调试，这些日志会自动轮转、不长期保留。

### 5. 处理过程中涉及的第三方

为实现核心功能，后端使用以下第三方服务：

- 一家第三方大语言模型服务——用于语法标注、翻译、出题。你的文本片段会发送到该服务做推理，**不会**被该服务保留。
- 一家第三方网页正文抽取服务——用于从你提交的网址抽取正文。
- 一家云端托管服务商——承载我们的后端运行。

我们不会把你的数据用于营销 / 数据分析目的发给第三方。

### 6. 数据安全

所有客户端 - 服务端通信走 HTTPS（TLS 1.2+）。你的学习数据（文章、已掌握词汇、进度等）
仅存于设备本地的 App sandbox，**卸载本应用即永久清除**。

### 7. 儿童隐私

本应用不面向 13 岁以下儿童，也不会主动收集 13 岁以下儿童的任何数据。

### 8. 你的权利

你可以：
- **删除所有数据**——卸载本应用即可（本地数据随之清除，服务端无你的可识别数据）。
- **随时停止使用**，无任何义务。

由于我们不收集可识别身份的数据，你没有账号可以删除，也没有数据可以从我们的服务器导出。

### 9. 政策变更

我们可能不定期更新本隐私政策。文档顶部的「最后更新」日期反映任何变更。
重大变更会在应用内提示。

### 10. 联系方式

如对本政策或你的数据有任何疑问，请联系：

**邮箱：kyoi.cn@gmail.com**
