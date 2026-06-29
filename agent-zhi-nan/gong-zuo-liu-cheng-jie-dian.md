# ワークフローノード

## はじめに

ワークフローシステムは、柔軟でスマート、かつモジュール化されたアシスタントを構築するための多様なノード設計を提供します。各ノードは、システムのロジック、ユーザーとのやり取り、バックエンドの統合を強化する上で、それぞれ異なる役割を担います。

<figure><img src="../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="80">項目</th><th width="160">ノード名</th><th>ワークフローでの用途</th></tr></thead><tbody><tr><td>1</td><td>ナレッジ検索</td><td>内部のナレッジベースやドキュメントデータベースから関連情報を検索します。</td></tr><tr><td>2</td><td>LLM</td><td>言語モデル（例：GPT-5.2 Thinking／GPT-5.2 Instant／Gemini 3）を使ってプロンプトを実行し、現在の入力に基づいて生成または推論の結果を出します。</td></tr><tr><td>3</td><td>応答</td><td>ユーザーが実際に見る内容を定義します — アシスタントの返信を出力して表示します。</td></tr><tr><td>4</td><td>注釈</td><td>キャンバス上に内部的な注釈やマークを追加します — 実際のロジックには接続されません。</td></tr><tr><td>5</td><td>変数ノード</td><td>前のステップの値を取得、保存、または変換し、後続のノードで利用できるようにします。</td></tr><tr><td>6</td><td>ガードレール</td><td>フロー内で内容をチェック・制限でき、個人情報の漏洩、情報セキュリティ、コンプライアンス関連のリスクを低減し、出力内容を利用規範や管理ニーズによりよく適合させます。</td></tr><tr><td>7</td><td>分類</td><td>あらかじめ定義したロジックまたはモデルベースの分類に従って、入力に自動的にタグを付けたり経路を誘導したりします。</td></tr><tr><td>8</td><td>分岐</td><td>データが各ノード間を流れる方向と順序を記述し、タスクを自動実行できるようにします。</td></tr><tr><td>9</td><td>マージ</td><td>異なる分岐の出力を同一のノードに集約し、まとめて後続のノードに渡して処理します。</td></tr></tbody></table>

### **ナレッジ検索**

内部のナレッジベースやドキュメントデータベースから関連情報を検索します。

<div align="center" data-with-frame="true"><figure><img src="../.gitbook/assets/image (29).png" alt="" width="375"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>ナレッジ検索</td><td>Input の内容（「/」を入力して query をユーザーの質問として選択）</td></tr><tr><td>2</td><td>ナレッジベース参照</td><td>必要なナレッジベースを選択します</td></tr><tr><td>3</td><td>検索パラメータ</td><td>「ナレッジベースのテスト - 検索パラメータ設定」を参照</td></tr></tbody></table>

### **LLM**

言語モデル（例：GPT-5.2 Thinking／GPT-5.2 Instant／Gemini 3）を使ってプロンプトを実行し、現在の入力に基づいて生成または推論の結果を出します。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (30).png" alt="" width="188"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>LLM 名</td><td>識別しやすいようにノード名を入力します</td></tr><tr><td>2</td><td>LLM パラメータ調整</td><td><a href="liao-tian-agent.md#can-shu">パラメータ</a> を参照</td></tr><tr><td>3</td><td>モデル</td><td>ノードで使用する言語モデルを変更します（2. のモデル設定と同じ）</td></tr><tr><td>4</td><td>コンテキスト</td><td>Input の内容（「/」を入力して query をユーザーの質問として選択）</td></tr><tr><td>5</td><td>ノードファイルの使用</td><td>LLM が前のノードからどのファイルを取得できるかを許可します</td></tr><tr><td>6</td><td>ファイル処理</td><td><a href="https://www.notion.so/3509f9da96be81ef9413d427bc2132c7?pvs=21">ファイル処理</a> を参照</td></tr><tr><td>7</td><td>ナレッジベースの有効化</td><td><a href="https://www.notion.so/3509f9da96be81d7b1bbe69f43f236d4?pvs=21">ナレッジベースのソース</a> を参照</td></tr><tr><td>8</td><td>Agent コラボレーション</td><td><a href="liao-tian-agent.md#agent-xie-zuo">Agent コラボレーション</a> を参照</td></tr><tr><td>9</td><td>スキル</td><td><a href="liao-tian-agent.md#ji-neng">スキル</a> を参照</td></tr><tr><td>10</td><td>記憶の参照</td><td>有効にすると、LLM は返信時に記憶ライブラリの記憶を参照します。記憶の保存方法は<a href="../ge-ren-she-ding/agent-memory.md"> Agent Memory</a> を参照してください</td></tr><tr><td>11</td><td>会話メモリ</td><td><a href="liao-tian-agent.md#can-shu">パラメータ</a> 内の会話メモリを参照</td></tr><tr><td>12</td><td>ツール</td><td><a href="liao-tian-agent.md#gong-ju">ツール</a> を参照</td></tr></tbody></table>

### **応答**

Response Node は **Agent の最終出力内容** を定義するために使われ、フローで整理し終えた結果を、ユーザーに返したり、後続システムへの出力としての応答にしたりする役割を担います。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (31).png" alt="" width="246"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>ノード名</td><td>識別しやすいようにノード名を入力します</td></tr><tr><td>2</td><td>説明</td><td>このノードの用途説明を記入できます</td></tr><tr><td>3</td><td>変数の設定</td><td>/ を入力して変数を設定します</td></tr></tbody></table>

### **注釈**

キャンバス上に内部的な注釈やマークを追加します — 実際のロジックには接続されません。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (32).png" alt="" width="249"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>ノード名</td><td>識別しやすいようにノード名を入力します</td></tr><tr><td>2</td><td>備考</td><td>後で識別できるよう備考内容を入力します</td></tr></tbody></table>

### **変数ノード**

前のステップの値を取得、保存、または変換し、後続のノードで利用できるようにします。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (33).png" alt="" width="375"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="200">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>変数（グローバル変数名）</td><td>書き込む<strong>グローバル変数のキー</strong>（例：<code>global.age</code>）を選択／指定するために使い、後続のフローノードで一貫した名前で読み取り・参照できるようにします。</td></tr><tr><td>2</td><td>変数内容（変数値）</td><td>そのグローバル変数の<strong>実際の値（Value）</strong>を設定し、後続のノードが直接利用できるようにします。</td></tr></tbody></table>

### ガードレール

あらかじめ定義したロジックまたはモデルベースの分類に従って、入力に自動的にタグを付けたり経路を誘導したりします。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (34).png" alt="" width="375"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>変数の設定</td><td>/ を入力して変数を設定します</td></tr><tr><td>2</td><td>ブロック／マスク</td><td>ガードレールの動作モードを選択します</td></tr><tr><td>3</td><td>カテゴリ</td><td>種類に応じてブロック／マスクする内容を選択します</td></tr></tbody></table>

### **分類**

あらかじめ定義したロジックまたはモデルベースの分類に従って、入力に自動的にタグを付けたり経路を誘導したりします。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (35).png" alt="" width="375"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>モデル</td><td>ノードで使用する言語モデルを変更します</td></tr><tr><td>2</td><td>コンテキスト</td><td>Input の内容（「/」を入力して query をユーザーの質問として選択）</td></tr><tr><td>3</td><td>カテゴリ</td><td>質問を分類します</td></tr></tbody></table>

### 分岐

データが各ノード間を流れる方向と順序を記述し、タスクを自動実行できるようにします。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (36).png" alt="" width="375"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>分岐</td><td>現在の分岐数を確認します</td></tr><tr><td>2</td><td>分岐の状態</td><td>現在の分岐の状態を確認します</td></tr></tbody></table>

### マージ

異なる分岐の出力を同一のノードに集約し、まとめて後続のノードに渡して処理します。

<div data-with-frame="true"><figure><img src="../.gitbook/assets/image (37).png" alt="" width="375"><figcaption></figcaption></figure></div>

<table><thead><tr><th width="80">項目</th><th width="160">機能名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>待機</td><td>待機中のノード数を確認します</td></tr><tr><td>2</td><td>入力状態</td><td>現在の入力状態を確認します</td></tr><tr><td>3</td><td>待機タイムアウト</td><td>待機タイムアウトを設定します</td></tr></tbody></table>
