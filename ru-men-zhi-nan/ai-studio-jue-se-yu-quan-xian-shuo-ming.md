---
description: AI Studio でユーザーが閲覧できる機能と操作は、アカウントが属するロールによって決まります。
---

# AI Studio のロールと権限の説明

## **AI Studio における機能ロールの種類**

システムには3種類の機能ロールがあらかじめ用意されています：

* **AI Studio 管理者：** プラットフォーム内のすべての機能メニューを閲覧でき、他のユーザーにナレッジベースやアシスタント機能の高度な操作権限を付与できます。
* **AI Studio コラボレーター：** プラットフォーム内のナレッジベース、能力、分析、テンプレート、Agent の機能メニューを閲覧でき、さまざまな分野やシーンに適したドキュメントナレッジベースおよび Agent を作成できます。
* **AI Studio ユーザー：** 企業内の一般ユーザーで、プラットフォーム内のナレッジベース、テンプレート、Agent の機能メニューを閲覧できます。

### **ロールの比較**

<table data-full-width="false"><thead><tr><th>機能モジュール第1階層</th><th>機能モジュール第2階層</th><th>AI Studio 管理者</th><th>AI Studio コラボレーター</th><th>AI Studio ユーザー</th></tr></thead><tbody><tr><td><strong>ワークスペース</strong></td><td></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>Agent</strong></td><td></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>ナレッジベース</strong></td><td></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>能力</strong></td><td>スキル</td><td>O</td><td>O</td><td>X</td></tr><tr><td></td><td>MCP</td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>テンプレート</strong></td><td>ワークフロー</td><td>O</td><td>O</td><td>O</td></tr><tr><td></td><td>プロンプト</td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>分析</strong></td><td>レポート</td><td>O</td><td>O（自分のみ）</td><td>O（自分のみ）</td></tr><tr><td></td><td>作業管理</td><td>O</td><td>X</td><td>X</td></tr><tr><td></td><td>監査ログ</td><td>O</td><td>X</td><td>X</td></tr><tr><td><strong>システム設定</strong></td><td>モデル</td><td>O</td><td>X</td><td>X</td></tr><tr><td></td><td>クォータ</td><td>O</td><td>X</td><td>X</td></tr><tr><td></td><td>構成</td><td>O</td><td>X</td><td>X</td></tr><tr><td></td><td>シークレット管理</td><td>O</td><td>X</td><td>X</td></tr><tr><td></td><td>タグ管理</td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

> 注意： 分析内のレポートはすべてのロールがアクセスできますが、すべてのアカウントの利用履歴を閲覧できるのは AI Studio 管理者のみです。
