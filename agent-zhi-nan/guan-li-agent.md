# Agent の管理

## **Agent の種類**

<figure><img src="../.gitbook/assets/image (136).png" alt=""><figcaption></figcaption></figure>

* **チャット Agent** ：基本的な質問応答を通じて、内部または外部の大規模言語モデルと直接やり取りします。
* **ワークフロー**：ワークフローを編成して複雑な利用シーンに対応できます。

> 注意：「チャット Agent」は企業内部の情報を検索して回答を生成することはできません。企業内部のナレッジを利用したい場合は「ナレッジ」型 Agent を使用してください。

## **Agent ライブラリの管理者を指名する**

<figure><img src="../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (138).png" alt=""><figcaption></figcaption></figure>

1. 画面左上の「…（その他）」ボタンをクリックします
2. 「指名」を選択します
3. ポップアップウィンドウの「ユーザーメニュー」をクリックしてユーザーを選択するか、テキストを入力して絞り込みます
4. 「Agent ライブラリロールメニュー」をクリックして、ユーザーに付与するロールを選択します
5. 「招待」ボタンをクリックして権限の割り当てを完了します
6. ユーザー行の右端の「削除」ボタンをクリックすると、ユーザーに付与した権限を削除できます

> ユーザーに割り当てたロールを変更するには、ユーザー行の「Agent ライブラリロール名」をクリックすると選び直せます

## Agent のエクスポート / インポート（JSON）

エクスポート / インポート機能は、Agent 設定のバックアップ、異なる環境間での設定の移行、類似 Agent の素早い複製による重複設定コストの削減に利用できます。

### Agent のエクスポート

<figure><img src="../.gitbook/assets/image (139).png" alt=""><figcaption></figcaption></figure>

1. Agent リストに移動するか、対象 Agent の編集ページに入ります。
2. エクスポートしたい Agent のテーブル上にマウスを移動します。
3. エクスポート（Export）ボタンを選択すると、システムが proas ファイルをダウンロードします。

### Agent のインポート

<figure><img src="../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (141).png" alt=""><figcaption></figcaption></figure>

1. 画面左上の「…（その他）」ボタンをクリックします
2. 「ファイルインポート」を選択します
3. 欄をクリックしてインポートするファイルを選択します
4. 「確定」をクリックして指定したファイルをインポートします

## 権限

リスト権限については [モジュール権限ロールの紹介 - Agent リスト権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#agent-qing-dan) を参照してください。

権限設定については [権限操作機能の紹介 - Root 権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#root-quan-xian) を参照してください。

### Agent 権限

ロール権限については [モジュール権限ロールの紹介 - Agent 権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#agent) を参照してください。

権限設定については [権限操作機能の紹介 - Object ロール権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#jue-se-quan-xian) を参照してください。
