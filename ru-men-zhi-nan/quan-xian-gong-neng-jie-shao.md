---
description: 本ページでは、各モジュールの権限機能について説明します。
---

# モジュール権限ロールの紹介

## **Agent モジュール権限**

### **Agent リスト**

以下の表は「Agent リスト」レベルでできることを示しています。「Agent リスト」は一つの管理範囲と考えることができます。項目を作成できるか、メンバーを管理できるか、すべての項目を閲覧／編集できるかは、この機能リストで付与されたロールによって決まります。

<figure><img src="../.gitbook/assets/image (112).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th width="183">ロール</th><th>Agent リスト管理者</th><th>Agent リストコラボレーター</th><th>Agent リストユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>Agent リストと Agent のすべての機能を操作できるロール</td><td>Agent リストのメンバー管理を補助する権限を付与されたロール</td><td>自分の Agent を作成・編集できるロール</td></tr><tr><td><strong>Agent の作成</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>Agent リストのメンバー管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>すべての Agent の閲覧</strong></td><td>O</td><td>X</td><td>X</td></tr><tr><td><strong>すべての Agent の編集</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### Agent

以下の表は「Agent」レベルでできることを示しています。この階層は通常、「Agent 管理者」または「Agent コラボレーター」がメンバーを管理し、適切な権限をコラボレーターやユーザーに割り当てます。

<figure><img src="../.gitbook/assets/image (113).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>Agent 管理者</th><th>Agent コラボレーター</th><th>Agent ユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>Agent の完全な制御権を持つ</td><td>Agent の利用やコンテンツ調整の管理を補助できる</td><td>ワークスペースで Agent を利用することのみができるロール</td></tr><tr><td><strong>ワークスペースで Agent を利用</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>Agent リストで Agent を閲覧</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>Agent メンバーの管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>Agent の編集</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>Agent の削除</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

## ナレッジベース**モジュール**権限

### ナレッジベースリスト

以下の表は「ナレッジベースリスト」レベルでできることを示しています。「ナレッジベースリスト」は一つの管理範囲と考えることができます。項目を作成できるか、メンバーを管理できるか、すべての項目を閲覧／編集できるかは、この機能リストで付与されたロールによって決まります。

<figure><img src="../.gitbook/assets/image (114).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>ナレッジベースリスト管理者</th><th>ナレッジベースリストコラボレーター</th><th>ナレッジベースリストユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>ナレッジベースとナレッジのすべての機能を操作できるロール</td><td>ナレッジベースのメンバー管理を補助する権限を付与されたロール</td><td>自分のナレッジを作成・編集できるロール</td></tr><tr><td><strong>ナレッジの作成</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>ナレッジベースのメンバー管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>すべてのナレッジの閲覧</strong></td><td>O</td><td>X</td><td>X</td></tr><tr><td><strong>すべてのナレッジの編集</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### ナレッジ

以下の表は「ナレッジ」レベルでできることを示しています。この階層は通常、「ナレッジ管理者」または「ナレッジコラボレーター」がメンバーを管理し、適切な権限をコラボレーターやユーザーに割り当てます。

<figure><img src="../.gitbook/assets/image (115).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>ナレッジ管理者</th><th>ナレッジコラボレーター</th><th>ナレッジユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>ナレッジの完全な制御権を持つ</td><td>ナレッジのコンテンツ調整の管理を補助できる</td><td>ナレッジの読み取りのみができるロール</td></tr><tr><td><strong>Agent でナレッジを追加可能</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>ナレッジベースリストでナレッジを閲覧</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>ナレッジメンバーの管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>ナレッジの編集</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>ナレッジの削除</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### **データセット**

ユーザー、グループ、または組織をデータセットに割り当てることで、管理者はどのユーザーが他の機能（Agent 設定、テスト、その他ナレッジベースに基づく機能など）でそのデータセットを利用できるかを制御できます。

権限設定を保存すると、選択したユーザー、グループ、または組織が、サポートされている機能でそのデータセットにアクセスして利用できるようになります。

<figure><img src="../.gitbook/assets/image (286).png" alt=""><figcaption></figcaption></figure>



## **スキルモジュール権限**

### **スキルリスト**

以下の表は「**スキル**リスト」レベルでできることを示しています。「**スキル**リスト」は一つの管理範囲と考えることができます。項目を作成できるか、メンバーを管理できるか、すべての項目を閲覧／編集できるかは、この機能リストで付与されたロールによって決まります。

<figure><img src="../.gitbook/assets/image (284).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>スキル リスト管理者</th><th>スキル リストコラボレーター</th><th>スキル リストユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>スキルリストとスキルのすべての機能を操作できるロール</td><td>スキルリストのメンバー管理を補助する権限を付与されたロール</td><td>自分のスキルを作成・編集できるロール</td></tr><tr><td><strong>スキルの作成</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>スキルメンバーの管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>すべてのスキルの閲覧</strong></td><td>O</td><td>X</td><td>X</td></tr><tr><td><strong>すべてのスキルの編集</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### **スキル**

以下の表は「スキル」レベルでできることを示しています。この階層は通常、「スキル管理者」または「スキルコラボレーター」がメンバーを管理し、適切な権限をコラボレーターやユーザーに割り当てます。

<figure><img src="../.gitbook/assets/image (285).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>スキル 管理者</th><th>スキル コラボレーター</th><th>スキル ユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>スキルの完全な制御権を持つ</td><td>スキルのコンテンツ調整の管理を補助できる</td><td>スキルの読み取りのみができるロール</td></tr><tr><td><strong>Agent でスキルを追加可能</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>スキルリストでスキルを閲覧</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>スキルメンバーの設定</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>スキルの編集</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>スキルの削除</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

## **MCP モジュール権限**

### **MCP リスト**

以下の表は「**MCP**リスト」レベルでできることを示しています。「**MCP**リスト」は一つの管理範囲と考えることができます。項目を作成できるか、メンバーを管理できるか、すべての項目を閲覧／編集できるかは、この機能リストで付与されたロールによって決まります。

<figure><img src="../.gitbook/assets/image (116).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>MCP リスト管理者</th><th>MCP リストコラボレーター</th><th>MCP リストユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>MCP リストと MCP のすべての機能を操作できるロール</td><td>MCP リストのメンバー管理を補助する権限を付与されたロール</td><td>自分の MCP を作成・編集できるロール</td></tr><tr><td><strong>MCP の作成</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>MCP メンバーの管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>すべての MCP の閲覧</strong></td><td>O</td><td>X</td><td>X</td></tr><tr><td><strong>すべての MCP の編集</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### **MCP**

以下の表は「MCP」レベルでできることを示しています。この階層は通常、「MCP 管理者」または「MCP コラボレーター」がメンバーを管理し、適切な権限をコラボレーターやユーザーに割り当てます。

<figure><img src="../.gitbook/assets/image (117).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>MCP 管理者</th><th>MCP コラボレーター</th><th>MCP ユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>MCP の完全な制御権を持つ</td><td>MCP のコンテンツ調整の管理を補助できる</td><td>MCP の読み取りのみができるロール</td></tr><tr><td><strong>Agent で MCP を追加可能</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>MCP リストで MCP を閲覧</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>MCP メンバーの設定</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>MCP の編集</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>MCP の削除</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### MCP ツール

ユーザー、グループ、または組織をツールに割り当てることで、管理者はどのユーザーが他の機能（Agent 設定、テスト、その他ツールに基づく機能など）でそのツールを利用できるかを制御できます。

権限設定を保存すると、選択したユーザー、グループ、または組織が、サポートされている機能でそのツールにアクセスして利用できるようになります。

<figure><img src="../.gitbook/assets/image (287).png" alt=""><figcaption></figcaption></figure>

## **ワークフローテンプレートモジュール権限**

### **ワークフローテンプレートリスト**

以下の表は「ワークフローテンプレートリスト」レベルでできることを示しています。「ワークフローテンプレートリスト」は一つの管理範囲と考えることができます。項目を作成できるか、メンバーを管理できるか、すべての項目を閲覧／編集できるかは、この機能リストで付与されたロールによって決まります。

<figure><img src="../.gitbook/assets/image (118).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>ワークフローテンプレートリスト管理者</th><th>ワークフローテンプレートリストコラボレーター</th><th>ワークフローテンプレートリストユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>ワークフローテンプレートリストとワークフローテンプレートのすべての機能を操作できるロール</td><td>ワークフローテンプレートリストのメンバー管理を補助する権限を付与されたロール</td><td>自分のワークフローテンプレートを作成・編集できるロール</td></tr><tr><td><strong>ワークフローテンプレートの作成</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>ワークフローテンプレートのメンバー管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>すべてのワークフローテンプレートの閲覧</strong></td><td>O</td><td>X</td><td>X</td></tr><tr><td><strong>すべてのワークフローテンプレートの編集</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### ワークフローテンプレート

以下の表は「ワークフローテンプレート」レベルでできることを示しています。この階層は通常、「ワークフローテンプレート管理者」または「ワークフローテンプレートコラボレーター」がメンバーを管理し、適切な権限をコラボレーターやユーザーに割り当てます。

<figure><img src="../.gitbook/assets/image (119).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>ワークフローテンプレート管理者</th><th>ワークフローテンプレートコラボレーター</th><th>ワークフローテンプレートユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>ワークフローテンプレートの完全な制御権を持つ</td><td>ワークフローテンプレートのコンテンツ調整の管理を補助できる</td><td>ワークフローテンプレートの読み取りのみができるロール</td></tr><tr><td><strong>ワークスペースでワークフローテンプレートを利用可能</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>ワークフローテンプレートリストでワークフローテンプレートを閲覧</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>ワークフローテンプレートメンバーの設定</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>ワークフローテンプレートの編集</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>ワークフローテンプレートの削除</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

## **プロンプトテンプレートモジュール権限**

### **プロンプトテンプレートリスト**

以下の表は「プロンプトテンプレートリスト」レベルでできることを示しています。「プロンプトテンプレートリスト」は一つの管理範囲と考えることができます。項目を作成できるか、メンバーを管理できるか、すべての項目を閲覧／編集できるかは、この機能リストで付与されたロールによって決まります。

<figure><img src="../.gitbook/assets/image (120).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>プロンプトテンプレートリスト管理者</th><th>プロンプトテンプレートリストコラボレーター</th><th>プロンプトテンプレートリストユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>プロンプトテンプレートリストとプロンプトテンプレートのすべての機能を操作できるロール</td><td>プロンプトテンプレートリストのメンバー管理を補助する権限を付与されたロール</td><td>自分のプロンプトテンプレートを作成・編集できるロール</td></tr><tr><td><strong>プロンプトテンプレートの作成</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>プロンプトテンプレートのメンバー管理</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>すべてのプロンプトテンプレートの閲覧</strong></td><td>O</td><td>X</td><td>X</td></tr><tr><td><strong>すべてのプロンプトテンプレートの編集</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

### プロンプトテンプレート

以下の表は「プロンプトテンプレート」レベルでできることを示しています。この階層は通常、「プロンプトテンプレート管理者」または「プロンプトテンプレートコラボレーター」がメンバーを管理し、適切な権限をコラボレーターやユーザーに割り当てます。

<figure><img src="../.gitbook/assets/image (121).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>プロンプトテンプレート管理者</th><th>プロンプトテンプレートコラボレーター</th><th>プロンプトテンプレートユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>プロンプトテンプレートの完全な制御権を持つ</td><td>プロンプトテンプレートのコンテンツ調整の管理を補助できる</td><td>プロンプトテンプレートの読み取りのみができるロール</td></tr><tr><td><strong>ワークスペースでプロンプトテンプレートを利用可能</strong></td><td>O</td><td>O</td><td>O</td></tr><tr><td><strong>プロンプトテンプレートリストでプロンプトを閲覧</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>プロンプトテンプレートメンバーの設定</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>プロンプトテンプレートの編集</strong></td><td>O</td><td>O</td><td>X</td></tr><tr><td><strong>プロンプトテンプレートの削除</strong></td><td>O</td><td>X</td><td>X</td></tr></tbody></table>

## **モデルモジュール権限**

{% hint style="info" %}
モデルモジュールは AI Studio 管理者のみが利用できるため、モジュールリストの権限設定はありません。
{% endhint %}

### **モデル**

以下の表は「モデル」レベルでできることを示しています。この階層は通常、「モデル管理者」がメンバーを管理し、適切な権限をコラボレーターやユーザーに割り当てます。

<figure><img src="../.gitbook/assets/image (306).png" alt=""><figcaption></figcaption></figure>

<table data-full-width="true"><thead><tr><th>ロール</th><th>モデルコラボレーター</th><th>モデルユーザー</th></tr></thead><tbody><tr><td><strong>説明</strong></td><td>モデルリストからモデルにアクセスし、モデルを利用できるロール</td><td>モデルの読み取りのみができるロール</td></tr><tr><td><strong>ワークスペースでモデルを使う Agent に質問応答</strong></td><td>O</td><td>O</td></tr><tr><td><strong>モデルリストでモデルを選択可能</strong></td><td>O</td><td>X</td></tr></tbody></table>
