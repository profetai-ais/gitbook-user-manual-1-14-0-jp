---
description: チャット Agent は、ユーザーが大規模言語モデルと直接やり取りできる機能で、ブレインストーミング、情報の要約、書式付きテキスト内容の生成などのタスクに適しており、機密データ漏洩の心配もありません。
---

# チャット Agent

## **Agent の作成**

<figure><img src="../.gitbook/assets/image (145).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (146).png" alt=""><figcaption></figcaption></figure>

1. 画面右上の「+ 作成」ボタンをクリックします
2. ポップアップウィンドウで「Agent タイプ」を選択します
3. 「名前」欄に名前を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](liao-tian-agent.md#duo-guo-yu-yan-she-ding) を参照してください
4. 「説明」欄に説明を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](liao-tian-agent.md#duo-guo-yu-yan-she-ding) を参照してください
5. 「タグ」メニューをクリックして、この Agent に付けるタグを選択します
6. 「モデル」メニューをクリックして、この Agent が使用する大規模言語モデルを選択します
7. 「保存」ボタンをクリックして追加を完了すると、システムが自動的に Agent 編集画面に入り、ユーザーが設定を完了できます

### 多言語設定 <a href="#duo-guo-yu-yan-she-ding" id="duo-guo-yu-yan-she-ding"></a>

<figure><img src="../.gitbook/assets/image (148).png" alt=""><figcaption></figcaption></figure>

1. 画面の「地球」ボタンをクリックすると自動翻訳が行われます。ユーザーは内容を手動で編集することもできます
2. 自動翻訳が完了したら「確定」ボタンをクリックして内容を保存します

> 注意：「モデル」メニューの大規模言語モデルの選択肢は、実際のインストール環境の構成を基準としてください。説明文書に示された選択肢は参考用です。

## チャット Agent の機能インターフェース

<figure><img src="../.gitbook/assets/image (149).png" alt=""><figcaption></figcaption></figure>

チャット Agent のホームページは主に次のいくつかの部分に分かれています：

1. **Agent 機能オプション**：機能オプションエリアには以下のリンクが含まれ、各リンクは対応する設定ページを開きます

| 名前        | 説明                  |
| --------- | ------------------- |
| 基本設定      | Agent のホームページを編集します        |
| 会話ログ      | この Agent の会話履歴を提供します     |
| メンバー管理      | この Agent のアクセス権限を管理します     |
| AI WEBAPP | この Agent のウェブ埋め込みを設定します     |
| API Key   | サードパーティアプリが安全に API を呼び出すための認証情報を提供します |

2. **基本情報**：Agent 名、作成・編集の日時と担当者、有効状態を確認できます
3. **アプリケーション設定：** Agent タイプに応じて、Agent の動作に関する設定を提供します

| 名前         | 説明                          |
| ---------- | --------------------------- |
| 推論パラメータ       | 応答生成の方法を制御します                   |
| ナレッジベース構成      | パラメータと利用可能なナレッジソースを選択します                |
| ツール         | 利用可能なツールを有効化・構成します                  |
| スキル         | Agent の能力を拡張するための機能            |
| Agent コラボレーション   | Agent が他の Agent と連携してタスクを実行できるようにします |
| Agent ウェルカムページ | 初期の会話内容を設定します                    |
| プロンプトテンプレート      | 再利用可能なプロンプトテンプレートを提供し、素早く使えるようにします         |
| ファイル処理方法     | アップロードファイルの処理方法を制御します                 |
| ガードレール         | コンテンツ出力を管理します                      |

4. **調整プレビュー：** ユーザーが質問応答の結果が期待どおりかをテストできるようにします

## **基本設定**

<figure><img src="../.gitbook/assets/image (150).png" alt=""><figcaption></figcaption></figure>

すべてのタイプの Agent のホームページは **基本設定** ブロックを共有しており、その中には **有効状態** のスイッチと、Agent の名前と説明を更新するための **設定** ボタンが含まれます。設定ボタンをクリックすると、以下のダイアログが表示されます：

1. **Agent の状態**：ユーザーは Agent の有効状態を編集でき、スイッチを切り替えると即座に状態が変わります。
2. **基本設定の編集**：最も基本的な名前、説明、および多言語翻訳を編集できます。

### Agent の状態設定

<figure><img src="../.gitbook/assets/image (151).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>

1. 状態欄をクリックしてインターフェースを開きます
2. 公開ボタンをクリックします
3. ワークスペースの URL をコピーできます
4. 会話ボタンをクリックすると、ワークスペースの会話を開きます
5. 未公開ボタンをクリックすると公開を取り消せます

## **アプリケーション設定**

### **推論パラメータ**

設定には「**パラメータ**」と「**システムプロンプト**」の2つのタブが含まれます。

#### **パラメータ**

ユーザーは「**パラメータ**」タブの項目を調整することで、Agent の返信動作を制御できます。

<figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="98">項目</th><th width="112">パラメータ</th><th width="238">説明</th><th>範囲と数値</th></tr></thead><tbody><tr><td>1</td><td>モデル</td><td>Agent 作成時に選択した既定のモデル。ここで変更できます</td><td>n/a</td></tr><tr><td>2</td><td>Temperature</td><td>返信の創造性を制御します。数値が高いほど応答は多様で創造的になり、低いほど応答は正確で一貫したものになります</td><td>0–2</td></tr><tr><td>3</td><td>Top P</td><td>ランダム性と多様性を制御します。数値が低いほど保守的で予測可能なテキストを生成し、高いほど多様な結果を生成します</td><td>0–1</td></tr><tr><td>4</td><td>最大トークン</td><td>最大出力長を制限します</td><td>必要に応じて設定</td></tr><tr><td>5</td><td>会話メモリ</td><td>質問応答の履歴を保存して一貫性を高めます（応答時間が遅くなる可能性があります）</td><td><code>0</code>はステートレスな応答を表します。<code>5-10</code>は一貫性と性能のバランスを取れます。記憶が多いほど速度は遅くなります。</td></tr></tbody></table>

#### 指示

ユーザーは「指示」タブを使ってプロンプトを定義し、Agent の言語、ロール、口調などを制御できます。

<figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

* **テンプレートを使ってプロンプトを追加する**

ユーザーはテンプレートから必要なアプリテンプレートを素早く追加できます。

<figure><img src="../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (156).png" alt=""><figcaption></figcaption></figure>

1. 空白の箇所から直接追加するか、プロンプトがある場合はマウスで追加したい位置を選択します。
2. 「テンプレート」ボタンをクリックしてテンプレートリストを開き、追加したいテンプレートの種類を選択します。
3. 対応するテンプレートが生成されます。追加されたテンプレートは選択反転の状態で生成されるので、自分のニーズに応じてさらに編集できます。
4. 「保存」ボタンをクリックして編集を完了します。

* **要件を入力してプロンプトを生成する**

プロンプト生成機能は「既存内容のリライト」または「空白からの生成」をサポートします。上部の赤い枠はリライトの基にする内容を任意で記入でき、下部の緑の入力欄に生成のガイドを記入すると結果が生成されます。

<figure><img src="../.gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

1. 下部の入力欄を選択し、プロンプトに対する要件を入力します。
2. キーボードの Enter キーまたは右側の生成ボタンを押し、AI が自動でテンプレートを生成するのを待ちます。
3. 自動生成が完了したら、自分のニーズに応じてさらに編集できます。
4. 「保存」ボタンをクリックして編集を完了します。

### ナレッジベース

#### ナレッジベースのソース

<figure><img src="../.gitbook/assets/image (187).png" alt=""><figcaption></figcaption></figure>

#### ナレッジベースのパラメータ

<figure><img src="../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

### **ツール**

ユーザーは設定で、Agent がアクセスできるツールを有効化／無効化できます。

<figure><img src="../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

#### **Session Memory**

<table><thead><tr><th width="250">ツール</th><th>説明</th></tr></thead><tbody><tr><td>KV 会話短期記憶</td><td>会話中に一時データをキーに基づいて正確に保存・取得できます。動的な変数（例：<code>ユーザー名</code>、<code>選択したプラン</code>）の追跡に非常に役立ちます。</td></tr><tr><td>graphiti - 記憶データの追加</td><td>エピソード的な情報（やり取りやイベントなど）をナレッジグラフに保存します。</td></tr><tr><td>graphiti - 記憶ノードの照会</td><td>エンティティの要約やノードレベルの記憶表現を取得します。</td></tr><tr><td>graphiti - 記憶ファクトの照会</td><td>記憶グラフ内で関連するファクトや構造化された関係を検索します。</td></tr><tr><td>graphiti - エンティティ関係の削除</td><td>グラフからエンティティ間に定義された関係を削除します。</td></tr><tr><td>graphiti - イベント断片の削除</td><td>記憶グラフ内の特定のイベント区間を削除します。</td></tr><tr><td>graphiti - エンティティ関係の取得</td><td>特定のエンティティに関連する構造化された関係を取得します。</td></tr><tr><td>graphiti - イベント断片の取得</td><td>最近の記憶エピソードを返し、会話や意思決定の背景を提供します。</td></tr><tr><td>graphiti - 記憶グラフのクリア</td><td>グラフベースの記憶システム全体をリセットします。</td></tr></tbody></table>

> 補足：Graphiti の詳細については、その公式サイトを参照してください。

#### **Academic Articles**

<table><thead><tr><th width="250">ツール</th><th>使用ガイド</th></tr></thead><tbody><tr><td>arXiv 論文検索</td><td>ユーザーが arXiv データベースから学術論文を検索できるようにします。</td></tr><tr><td>Google Scholar 検索</td><td>Google Scholar を使って学術記事や引用を検索します。</td></tr></tbody></table>

#### **Web Search**

<table><thead><tr><th width="250">ツール</th><th>使用ガイド</th></tr></thead><tbody><tr><td>Serper - ウェブコンテンツ抽出</td><td>ウェブページの URL から読み取り可能な内容を抽出します。</td></tr><tr><td>Serper - Google 検索</td><td>Google 検索を実行し、要約結果を返します。</td></tr><tr><td>Serper - 特許検索</td><td>公開された特許や関連文書を検索します。</td></tr><tr><td>Serper - 画像検索</td><td>テキストクエリに基づいて画像を検索します。</td></tr><tr><td>Serper - 論文検索</td><td>Google Scholar 風のソースを使って学術論文を照会します。</td></tr><tr><td>Serper - ニュース検索</td><td>テキストクエリに基づいてニュースを検索します。</td></tr><tr><td>Serper - 地図情報検索</td><td>テキストクエリに基づいて地図を検索します。</td></tr></tbody></table>

> 補足：Serper の詳細については、その公式サイトを参照してください。

#### **Code**

<table><thead><tr><th width="250">ツール</th><th>使用ガイド</th></tr></thead><tbody><tr><td>Python コードの実行</td><td>Python スクリプトやロジックを実行し、数学、データ解析、自動化などのタスクをサポートします。</td></tr></tbody></table>

#### **Document Handling**

<table><thead><tr><th width="250">ツール</th><th>使用ガイド</th></tr></thead><tbody><tr><td>ドキュメントのプレビュー</td><td>アップロードしたドキュメントをプラットフォーム内で読み取り可能な形式で表示します。</td></tr><tr><td>ドキュメントを markdown に変換</td><td>ドキュメントを Markdown 形式に変換します。</td></tr></tbody></table>

#### **Other**

<table><thead><tr><th width="250">ツール</th><th>使用ガイド</th></tr></thead><tbody><tr><td>現在時刻の取得</td><td>リクエストを発行した時点の現在のシステム時刻を返します。</td></tr><tr><td>簡単な数式計算</td><td>プロンプト内で簡単な算術演算を実行します。</td></tr><tr><td>動的思考チェーン（Sequential Thinking）</td><td>複雑な問題を段階的な思考に分解し、修正や分岐を選択できます。計画、トラブルシューティング、構造化された推論に適しています。</td></tr></tbody></table>

### スキル

<figure><img src="../.gitbook/assets/image (170).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (169).png" alt=""><figcaption></figcaption></figure>

異なるスキルを設定することで、Agent はデータアクセス、ツール操作、フロー実行、特定タスクの拡張など、より多くの機能やタスク処理シーンに対応できます。ユーザーはニーズに応じて対応するスキルを構成し、Agent の活用の柔軟性とタスク処理能力を高められます。

### Agent コラボレーション

この機能を使うと、ユーザーは複数の Agent 間の協力関係を構築でき、異なる職責に応じて分担してタスク内容を処理し、フローの柔軟性と全体的なタスク処理効率を高められます。

<figure><img src="../.gitbook/assets/image (172).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (171).png" alt=""><figcaption></figcaption></figure>

### ガードレール

ガードレールはコンテンツ出力を管理するための機能で、フロー内で内容をチェック・制限でき、個人情報の漏洩、情報セキュリティ、コンプライアンス関連のリスクを低減し、出力内容を利用規範や管理ニーズによりよく適合させます。

<figure><img src="../.gitbook/assets/image (173).png" alt=""><figcaption></figcaption></figure>

### **会話パネル**

会話パネルには、プロンプトテンプレート、ウェルカムページ、操作メニューの設定があります。

#### **プロンプトテンプレート**

ユーザーは、既存またはお気に入りに追加したアプリテンプレート（プロンプトテンプレート）を Agent に紐づけ、必須項目を記入することで質問応答を高速化できます。

<figure><img src="../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>

#### **ウェルカムページ**

**クイック質問**

ユーザーは既定の会話内容を自分で設定でき、Agent が会話開始前に直接クリックできる質問の方向性を提示することで、ユーザーがより素早くやり取りを始められるよう支援します。

<figure><img src="../.gitbook/assets/image (329).png" alt=""><figcaption></figcaption></figure>

**開始メッセージ**

Agent の初期挨拶メッセージを設定します。ユーザーがこの Agent を選んで会話を始めると、Agent が会話の冒頭として自動的にこのメッセージを先に送信します。

<figure><img src="../.gitbook/assets/image (330).png" alt=""><figcaption></figcaption></figure>

#### **操作メニュー**

**ファイル処理**

**ファイル処理** 設定では、Agent がワークスペースでアップロードされたファイルをどう処理するかをユーザーが定義できます。Agent が PDF、DOCX、画像などのファイルから内容を読み取り、変換、抽出する必要がある場合に特に便利です。

<figure><img src="../.gitbook/assets/image (331).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="109.5555419921875">オプション</th><th width="101.111083984375">MCP ツールに表示</th><th width="83.4444580078125">LLM に表示</th><th>説明</th><th>使用シーンの例</th></tr></thead><tbody><tr><td>なし</td><td>X</td><td>X</td><td>ファイルはアップロードされますが、LLM にも MCP ツールにも表示されません。開かれたり読み取られたりしません。</td><td>– –</td></tr><tr><td>LLM</td><td>O</td><td>X</td><td>ファイルは処理のため MCP ツールに渡されますが、LLM には渡されません。<br>サポートするファイル形式：<br>ドキュメント：PDF、DOCX、DOC、PPTX、PPT<br>画像：JPG、JPEG、PNG、GIF、BMP</td><td>CSV や PDF からデータを抽出したいが、AI が生成する論評は不要な場合に役立ちます。</td></tr><tr><td>ツール処理</td><td>X</td><td>O</td><td>ファイルは画像に変換され、参照用として LLM にのみ表示されます。<br>注意： このオプションを有効にするには、さらにツール > Document Processing で File Preview を選択する必要があります。</td><td>図表の関係が重要なスキャン文書や視覚レイアウトに適しています。</td></tr><tr><td>すべて</td><td>O</td><td>O</td><td>ファイルは LLM の参照用に変換されると同時に、MCP ツールで処理されます。<br>注意： このオプションを有効にするには、さらにツール > Document Processing で File Preview を選択する必要があります。</td><td>視覚レイアウトと構造化データの両方を読み取る必要がある請求書やフォームに最適です。</td></tr></tbody></table>

**Canvas**

有効にすると、会話入力メニューに Canvas オプションが表示されます。

Agent 作成時、Canvas スイッチは既定でオンになっています。

<figure><img src="../.gitbook/assets/image (332).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (333).png" alt=""><figcaption></figcaption></figure>

## **調整プレビュー**

このブロックを使って Agent の返信をテストし、それに基づいて設定を調整します。

> 注意： 調整プレビューでアップロードまたは生成したファイルは30分間のみ保持されます。

<figure><img src="../.gitbook/assets/image (174).png" alt=""><figcaption></figcaption></figure>

### **調整プレビュー** でのファイルアップロード方法

* 入力欄のプラス（+）をクリックしてファイルをアップロードできます

<figure><img src="../.gitbook/assets/image (175).png" alt=""><figcaption></figcaption></figure>

* ファイルをドラッグ＆ドロップでアップロードする方法もサポートしています

<figure><img src="../.gitbook/assets/image (176).png" alt=""><figcaption></figcaption></figure>

## 記憶

記憶機能は、ユーザーが Agent のために再利用可能な記憶内容を作成するのを支援し、Agent がタスクを実行したり質問に応答したりする際に、あらかじめ設定した背景情報、利用シーン、処理フローを参照できるようにします。

ユーザーは Agent の記憶ページで作成済みの記憶リストを確認でき、有効状態、名前、説明、利用シーンによって各記憶の用途を素早く識別できます。記憶は特定のタスクフロー、判断ルール、前提条件、操作手順、注意事項を保存するのに使え、Agent が以降のやり取りで一貫した処理ロジックを維持するのを支援します。

<figure><img src="../.gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

### 記憶の作成

<figure><img src="../.gitbook/assets/image (180).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (181).png" alt=""><figcaption></figcaption></figure>

1. Agent ページに入ります。左側のサブメニューで「記憶」をクリックします。
2. 右上の「作成」ボタンをクリックします。
3. 記憶の基本情報を記入します：
   * 名前：記憶の名前を入力します。
   * 説明：記憶の説明を入力します。
   * 適用シーン：この記憶が適用される利用シーンを入力します。
   * 内容：詳細な内容を入力します。Markdown 形式で編集できます。
4. 内容に誤りがないことを確認したら、「作成」をクリックして作成を完了します。

### 記憶の詳細内容を確認する

<figure><img src="../.gitbook/assets/image (179).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

1. 記憶リストに入ります。
2. 確認したい記憶の名前をクリックします。
3. システムが右側に詳細内容パネルを開きます。
4. ユーザーは記憶の名前、有効状態、説明、利用シーン、完全な内容を確認できます。内容が長い場合は、右側パネルで上下にスクロールして確認できます。

### 記憶の有効化と無効化

#### 記憶の有効化ルール

記憶機能には、全体機能のスイッチと、記憶1件ごとの有効状態が含まれます。

<figure><img src="../.gitbook/assets/image (182).png" alt=""><figcaption></figcaption></figure>

スイッチがオンの場合、この Agent は記憶機能を使用できます。ユーザーは記憶リストで個別に各記憶を有効化または無効化できます。

スイッチがオフの場合、この Agent は記憶機能を使用しません。記憶リストに作成済みの記憶が残っていても、Agent はそれらの記憶内容を適用しません。

#### 記憶1件ごとの有効化と無効化

<figure><img src="../.gitbook/assets/image (183).png" alt=""><figcaption></figcaption></figure>

記憶リストの「有効」欄は、記憶1件が有効かどうかを表示するために使います。記憶の全体スイッチがオンの場合に限り、有効な記憶が Agent の応答やタスク処理時の参照内容として使われます。

ユーザーは、一時的に使用しない記憶をニーズに応じて無効化し、内容を保持したまま Agent に適用させないようにできます。後で再び使用する必要がある場合は、再度有効化できます。

## **会話ログ**

会話履歴には、この Agent のすべての会話履歴が保存されます。管理者はタイトル、ユーザー、日付範囲で履歴を絞り込めます。履歴には処理フローが含まれ、エラーが発生したり応答が遅かったりした場合、管理者は処理の詳細を確認して問題を診断できます。

<figure><img src="../.gitbook/assets/image (184).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (185).png" alt=""><figcaption></figcaption></figure>

## **Web App**

Agent は次のように、質問応答サービスを提供するためにウェブページに埋め込むことができます：

<figure><img src="../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

Agent をウェブサイトに埋め込むには、この機能を使ってフロントエンドの埋め込みコードを生成します。

### **Web App の追加**

<figure><img src="../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (82).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (83).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

1. 「Agent 機能リスト」内の Web App に入ります
2. 「+」をクリックして _作成_ Web App ダイアログを開きます
3. 「名前」欄に名前を入力した後、右側のボタンをクリックして多言語ラベルを作成します
4. 「説明」欄に説明を入力した後、右側のボタンをクリックして多言語ラベルを作成します
5. 「保存」をクリックして完了します
6. 新しい Web App がリストに表示されます。「操作」メニューを使って「編集」、「有効期限の設定」、「削除」を行います
7. Web App 名をクリックして情報ページにアクセスし、「埋め込みコード」の確認、_アプリケーション言語_、_リクエストとトークンの制限_ などを設定します

> Note：各 Agent は複数の API キーと対応する埋め込みコードを持つことができ、異なる Web App インスタンスの有効期限や利用制限を個別に管理できます。

## API Key

API Key は本人確認のためのアクセスキーで、システムが Agent API を呼び出す際に、リクエストの送信元を識別し、対応する権限と利用クォータを適用できるようにします。API Key は外部に流出しないよう適切に保管してください。キーが漏洩した疑いがある場合は、ただちに交換し、そのキーを使用しているすべての連携設定を更新することをお勧めします。

<figure><img src="../.gitbook/assets/image (85).png" alt=""><figcaption></figcaption></figure>

### API Key の追加

<figure><img src="../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>

1. 「Agent 機能リスト」内の API Key に入ります
2. 「+」をクリックして _作成_ API Key ダイアログを開きます
3. API Key の名前を入力します
4. Rate Limit を有効にするかどうかを選択し、数値を設定します
5. 必要に応じて、API Key の有効期限を設定できます
6. 「保存」ボタンをクリックします

> 注意： 保存後、ID と API キーをただちにコピーして、紛失しないようにしてください。

### Endpoint のコピー

Endpoint は Agent API のサービス入口の位置（URL）です。システムは対応する機能を実行するために、API リクエストをこの位置に送ります。利用シーンに応じて正しい Endpoint（例：テスト環境または本番環境）を選択し、リクエストを誤った環境に送ったり接続に失敗したりしないようにしてください。

Endpoint のコピーボタンは検索ボックスの横にあり、コピーボタンをクリックすると URL をコピーできます。URL をコピーする際は、どの環境にいるかに注意してください。

<figure><img src="../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>
