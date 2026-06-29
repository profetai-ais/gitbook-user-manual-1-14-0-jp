---
description: 本ページは、システムに必要なシークレット（API Key）を集中管理するために使います。このページでシークレットの追加、確認、削除ができ、システムサービスが安全かつ正しく動作することを確保します。
---

# シークレット管理

## ページガイド

「Key Management」ページに入ると、現在作成済みのシークレット一覧が表示されます。各欄の説明は次のとおりです：

<figure><img src="../.gitbook/assets/image (9) (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="210">名前</th><th>説明</th></tr></thead><tbody><tr><td>Type</td><td>シークレットの種類（例：SERPER、LiteLLM）。このキーが対応するサービスの種類を表します</td></tr><tr><td>Name</td><td>シークレット名。この API Key の用途を識別するために使います</td></tr><tr><td>Key</td><td>API Key の値。セキュリティ上の理由からマスク表示のみされます</td></tr><tr><td>Tenant ID</td><td>所属するテナントの識別子</td></tr><tr><td>Expire Date</td><td>シークレットの有効期限</td></tr><tr><td>Creator</td><td>作成者</td></tr><tr><td>Created Date</td><td>作成時刻</td></tr><tr><td>Modified Date</td><td>最終更新時刻</td></tr><tr><td>Actions</td><td>操作機能。現在は削除（ゴミ箱アイコン）を提供しています</td></tr></tbody></table>

## シークレットの追加

<figure><img src="../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

1. 右上の「+」をクリックすると、シークレット追加の設定ウィンドウが開きます。以下の設定を順に完了してください：
2. Type：シークレットの種類を選択します。
3. Name：この API Key の識別名を入力します。後で管理しやすいよう、具体的な用途（例：`litellm api key`）を記入することをお勧めします。
4. API Key：実際の API キーの内容を入力します。
   * 欄は既定で非表示になっています
   * 右側の「目」アイコンで表示／非表示を切り替えられます
5. 送信の確認：設定が完了したら「Ok」をクリックしてシークレットを保存します。保存しない場合は「キャンセル」をクリックして操作を取り消せます。

## シークレットの削除

<figure><img src="../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

1. その行の右端の Actions 欄にあるゴミ箱アイコンをクリックします
2. 確認をクリックすると削除が実行され、そのシークレットはただちに一覧から削除されます

### **注意事項**

* **削除したシークレットは復元できません**
* その API Key がシステムやフローで使用中の場合、削除すると関連機能が正常に動作しなくなる可能性があります
* 削除前に、そのキーがいかなるサービスやフローからも参照されていないことを確認することをお勧めします
