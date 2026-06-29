# MCP

## はじめに

**MCP ツール**ページは、統合済みで LLM の能力を拡張できる（リアルタイム検索、ファイル解析など）すべてのツールの更新記録を提供します。

ユーザーは次のことができます：

* ツールのグループ、名前、説明、作成者、作成日時、変更日を**確認**する
* 開発者が追加したツールを**追跡**する
* 利用可能なツールとその機能を**参照**する

<figure><img src="../.gitbook/assets/image (232).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (233).png" alt=""><figcaption></figcaption></figure>

## MCP サーバーの追加

### 手動でサーバーを追加する

<figure><img src="../.gitbook/assets/image (326).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (325).png" alt=""><figcaption></figcaption></figure>

1. MCP タブに移動します
2. 追加ボタンをクリックし、External を選択します
3. サーバー名を入力します
4. エンドポイントを入力します
5. HTTP または SSE タイプを選択します
6. ヘッダー情報を入力します。複数件入力できます
7. 送信をクリックして作成を完了します

### MCPHub からインポートする

<figure><img src="../.gitbook/assets/image (327).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (328).png" alt=""><figcaption></figcaption></figure>

1. MCP タブに移動します
2. 追加ボタンをクリックし、MCPHub を選択します
3. サーバー名を入力します
4. 対象フォルダーを選択します
   * フォルダーのソースは、ユーザーが MCPHub 内で作成した項目です。リストに内容がない場合は、先に MCPHub で構築してください
5. インポートをクリックして作成を完了します





## 権限

リスト権限については [モジュール権限ロールの紹介 - MCP リスト権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#mcp-qing-dan) を参照してください。

権限設定については [権限操作機能の紹介 - Root 権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#root-quan-xian) を参照してください。

### MCP 権限

ロール権限については [モジュール権限ロールの紹介 - MCP 権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#mcp) を参照してください。

権限設定については [権限操作機能の紹介 - Object ロール権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#jue-se-quan-xian) を参照してください。

### MCP ツール権限

ロール権限については [モジュール権限ロールの紹介 - MCP ツール権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#mcp-gong-ju) を参照してください。

権限設定については [権限操作機能の紹介 - Object アクセス権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#cun-qu-quan-xian) を参照してください。
