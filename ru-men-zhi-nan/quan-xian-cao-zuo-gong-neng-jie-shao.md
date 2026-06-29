---
description: 本ページでは、Root 権限と Object 権限の操作方法を紹介します。
---

# 権限操作機能の紹介

## **Root 権限**

### **開く場所**

Root の権限設定はモジュール右上の「その他」ボタンにあり、クリックすると権限管理ウィンドウが開きます。

<figure><img src="../.gitbook/assets/image (352).png" alt=""><figcaption></figcaption></figure>

### ページガイド

<figure><img src="../.gitbook/assets/image (349).png" alt=""><figcaption></figcaption></figure>

| 項目 | 操作名称    | 説明                             |
| -- | ------- | ------------------------------ |
| 1  | ユーザー選択   | 名前またはアカウントで検索してユーザーを追加します                   |
| 2  | 権限選択    | 設定したいリスト権限を選択します                     |
| 3  | 追加済みユーザー | 追加済みユーザーの情報とその権限設定を確認し、権限の調整やユーザーの削除ができます |

### **メンバーの追加**

<figure><img src="../.gitbook/assets/image (351).png" alt=""><figcaption></figcaption></figure>

1. キーワードを入力して追加したいユーザーを検索します
2. 追加する権限を設定します
3. 「追加」をクリックして設定を完了します。権限設定は相手がページを更新した後に有効になります

### **メンバー権限の調整**

<figure><img src="../.gitbook/assets/image (362).png" alt=""><figcaption></figcaption></figure>

1. 権限を調整したい対象ユーザーを見つけます
2. 右側のドロップダウンメニューをクリックして権限を調整します

### **メンバーの削除**

<figure><img src="../.gitbook/assets/image (363).png" alt=""><figcaption></figcaption></figure>

1. 削除したい対象ユーザーを見つけます
2. 右側のドロップダウンメニューをクリックして「削除」を選択します

## Object 権限

機能ごとに Object 権限は異なる権限モードを採用している場合があります。一般的なモードには、ロール型権限とアクセス権限の2種類があります。

### **開く場所**

権限設定はモジュール内のオブジェクトにあります。対象オブジェクトをクリックし、内ページの「権限」タブを選択すると権限管理ページを確認できます。ここでは Agent モジュールを例にしています。

<figure><img src="../.gitbook/assets/image (353).png" alt=""><figcaption></figcaption></figure>

### ロール権限

ロール権限は、ロールごとにユーザーが実行できる操作を区別します。各オブジェクトには2～3種類の権限ロールを設定でき、作成者は「権限」を通じて他のユーザーにアクセス権限を付与できます。より高い権限を持つユーザーは通常、オブジェクトの設定管理、コンテンツの調整、権限付与対象の維持ができます。より低い権限を持つユーザーは、そのオブジェクトの閲覧や利用のみができる場合があります。

一般的なケースには次のものがあります：

* そのオブジェクトを管理できる
* そのオブジェクトを編集できる
* そのオブジェクトを閲覧または利用できる

> 注意： 実際のロール名と操作可能な範囲は機能の設計によって異なります（ロールの定義は[モジュール権限の紹介](quan-xian-gong-neng-jie-shao.md)を参照してください）。

### ページガイド

<figure><img src="../.gitbook/assets/image (355).png" alt=""><figcaption></figcaption></figure>

| 項目 | 操作名称 | 説明                            |
| -- | ---- | ----------------------------- |
| 1  | テーブル編集 | テーブルの表示方法をユーザーが編集できるようにします                |
| 2  | 更新   | クリックするとリストを更新します                       |
| 3  | コンテンツフィルター | 指定したコンテンツを詳細にフィルタリングします                      |
| 4  | 一括削除 | 項目をチェックすると左上に削除ボタンが表示され、複数の項目を削除できます |
| 5  | 検索欄 | 名前を検索します                         |
| 6  | 招待   | 組織 / メンバーを招待します                     |
| 7  | 操作   | 自分のロールを移譲、または選択したユーザーを削除します               |

#### **メンバーの追加**

<figure><img src="../.gitbook/assets/image (356).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (357).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (358).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (360).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (361).png" alt=""><figcaption></figcaption></figure>

1. 「追加」をクリックして_新規メンバー追加_ダイアログを開きます
2. 入力欄で組織またはユーザーを検索できます
3. 対応する権限を選択します
4. ここでは組織／ユーザーを選択する方法が2つあります
   * 組織検索を使用してクリックします
   * キーワードを入力すると対応する組織／ユーザーが表示され、右側の階層ボタンをクリックしてロールの階層を確認できます
5. 対象の組織／ユーザーを選択した後、タグをクリックして閲覧メニューを開き、組織階層およびロール内のすべてのユーザーを確認できます
6. 「追加」ボタンをクリックして招待を完了します

#### **メンバー権限の調整**

<figure><img src="../.gitbook/assets/image (364).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (365).png" alt=""><figcaption></figcaption></figure>

1. 権限を調整したい対象の組織／ユーザーを見つけ、編集ボタンをクリックします
2. 権限を調整します
3. 「保存」をクリックして設定を完了します

#### **オーナーの移譲**

<figure><img src="../.gitbook/assets/image (366).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (367).png" alt=""><figcaption></figcaption></figure>

1. オーナー権を移譲したい対象ユーザーを見つけ、権限移譲ボタンをクリックします
2. 移譲するユーザーの情報を確認します
3. 「移譲」をクリックして設定を完了します

> 注意：&#x20;
>
> 1. オーナー移譲機能はユーザーに対してのみ使用でき、組織にオーナーを移譲することはできません。
> 2. オーナーを移譲すると、object のオーナーと作成者は自動的に新しいユーザーに変更されますが、あなたの object 権限は移譲前の設定のまま維持されます。

#### **メンバーの削除**

<figure><img src="../.gitbook/assets/image (368).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>

1. 削除したい対象の組織／ユーザーを見つけ、削除ボタンをクリックします
2. 対象を削除するか再度確認し、削除ボタンをクリックします

### アクセス権限

アクセス権限は組織または個人ユーザーに付与できます。組織に付与した場合、その組織内のすべてのユーザーがそのデータの利用権限を持ちます。ここではナレッジベースのデータセットを例にしています。

{% hint style="info" %}
アクセス権限の設定を持つ object は、AI Studio 内では現在**ナレッジベースのデータセット**および **MCP の MCP ツール**があります。
{% endhint %}

#### **メンバーの追加**

<figure><img src="../.gitbook/assets/image (371).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (373).png" alt=""><figcaption></figcaption></figure>

1. 「ナレッジ設定メニュー」内の _データセットアクセス権限_ 項目をクリックします
2. ボタンをクリックしてデータセットに権限を一括追加します
3. 「データセット」エリアで権限を設定するファイルを選択します
4. 右側エリアで「組織」タブをクリックし、権限を付与する組織階層をチェックします
5. 右側エリアで「ユーザー」タブをクリックし、権限を付与するユーザーを選択します
6. 「ユーザーメニュー」で追加するユーザーを検索します
7. 組織とユーザーの変更を完了したら「ok」ボタンをクリックして設定を保存します

#### **メンバーの削除**

<figure><img src="../.gitbook/assets/image (375).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (374).png" alt=""><figcaption></figcaption></figure>

1. 削除したいデータセットの編集ボタンをクリックします
2. 削除する組織またはユーザーを選択し、削除ボタンをクリックします
3. 「保存」をクリックして設定を完了します
