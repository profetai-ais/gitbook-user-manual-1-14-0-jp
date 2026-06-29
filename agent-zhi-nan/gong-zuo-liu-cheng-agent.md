---
description: ワークフロー Agent では、ユーザーがフローを構築する形で、AI Studio が提供する機能コンポーネントを通じて Agent がユーザーの複雑なタスクをどう完了するかを設計できます。
---

# ワークフロー Agent

## **ワークフロー Agent の作成**

<figure><img src="../.gitbook/assets/image (145).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (189).png" alt=""><figcaption></figcaption></figure>

1. 画面右上の「+ 作成」ボタンをクリックします
2. ポップアップウィンドウで「Agent タイプ」を _ワークフロー_ に選択します
3. 「名前」欄に名前を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-agent.md#duo-guo-yu-yan-she-ding) を参照してください
4. 「説明」欄に説明を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-agent.md#duo-guo-yu-yan-she-ding) を参照してください
5. 「Workflow Template」メニューをクリックしてワークフローテンプレートを選択します
6. 「保存」ボタンをクリックして追加を完了すると、システムが自動的に Agent 編集画面に入り、ユーザーが設定を完了できます

### 多言語設定

<figure><img src="../.gitbook/assets/image (148).png" alt=""><figcaption></figcaption></figure>

1. 画面の「地球」ボタンをクリックすると自動翻訳が行われます。ユーザーは内容を手動で編集することもできます
2. 自動翻訳が完了したら「確定」ボタンをクリックして内容を保存します

> 注意：ワークフローメニューのワークフローテンプレートの選択肢は、実際のインストール環境の構成を基準としてください。説明文書に示された選択肢は参考用です。

## ワークフロー Agent の機能インターフェース

ワークフロー Agent のホームページは、次のいくつかの主要エリアに分かれています：

<figure><img src="../.gitbook/assets/image (191).png" alt=""><figcaption></figcaption></figure>

1.  **Agent 機能オプション：** Agent の機能設定へのリンクを提供します

    機能オプションエリアには以下の機能リンクが含まれ、クリックすると対応する設定ページが表示されます：

<table><thead><tr><th width="250">名前</th><th>説明</th></tr></thead><tbody><tr><td>基本設定</td><td>Agent のホームページを編集します</td></tr><tr><td>フロー設定</td><td>Agent のワークフローを編集します</td></tr><tr><td>会話ログ</td><td>この Agent の会話履歴を提供します</td></tr><tr><td>メンバー管理</td><td>この Agent のアクセス権限を管理します</td></tr><tr><td>AI WEBAPP</td><td>この Agent のウェブ埋め込みを設定します</td></tr><tr><td>API Key</td><td>サードパーティアプリが安全に API を呼び出すための認証情報を提供します</td></tr></tbody></table>

2. **基本情報**：Agent 名、説明、有効状態を編集できます
3. **アプリケーション設定：** Agent タイプに応じて、Agent の動作に関する設定を提供します

<table><thead><tr><th width="250">名前</th><th>説明</th></tr></thead><tbody><tr><td>ウェルカムページ</td><td>Agent の質問設定を行います</td></tr><tr><td>プロンプトテンプレート</td><td>既存のプロンプトテンプレートを追加し、後で使えるようにします</td></tr><tr><td>ファイル処理方法</td><td>アップロードファイルの処理方法を制御します</td></tr></tbody></table>

4. **調整プレビュー：** ユーザーが質問応答の結果が期待どおりかをテストできるようにします

## **基本設定**

すべてのタイプの Agent のホームページは「基本設定」ブロックを共有しており、その中には「有効状態」のスイッチと、Agent の名前と説明を更新するための「設定」ボタンが含まれます。設定ボタンをクリックすると、以下のダイアログが表示されます：

<figure><img src="../.gitbook/assets/image (192).png" alt=""><figcaption></figcaption></figure>

1. **Agent の状態**：ユーザーは Agent の有効状態を編集でき、スイッチを切り替えると即座に状態が変わります。
2. **基本設定の編集**：最も基本的な名前、説明、および多言語翻訳を編集できます。

### Agent の状態設定

<figure><img src="../.gitbook/assets/image (192).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (193).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (194).png" alt=""><figcaption></figcaption></figure>

1. 状態欄をクリックしてインターフェースを開きます
2. 公開ボタンをクリックします
3. ワークスペースの URL をコピーできます
4. 会話ボタンをクリックすると、ワークスペースの会話を開きます
5. 未公開ボタンをクリックすると公開を取り消せます

## **アプリケーション設定**

Agent タイプに応じて Agent の動作に関する設定を提供します。以下では _ワークフロー Agent_ のアプリケーション設定を説明します。

### **プロンプトテンプレート**

作成済みまたはお気に入りに追加したアプリテンプレート（プロンプトテンプレート）を Agent に紐づけることができ、使用時には必要な情報を記入するだけで質問応答フローを高速化できます。

<figure><img src="../.gitbook/assets/image (195).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (197).png" alt=""><figcaption></figcaption></figure>

### **ウェルカムページ**

ユーザーは既定の会話内容を自分で設定でき、Agent が会話開始前に直接クリックできる質問の方向性を提示することで、ユーザーがより素早くやり取りを始められるよう支援します。

<figure><img src="../.gitbook/assets/image (196).png" alt=""><figcaption></figcaption></figure>

## **調整プレビュー**

ユーザーはこのエリアで Agent の動作や返信内容をテストし、返信に基づいて Agent の構成を調整できます。

<figure><img src="../.gitbook/assets/image (198).png" alt=""><figcaption></figcaption></figure>

## ワークフロー設定

Agent 機能オプションの「ワークフロー設定」は Agent のワークフローを編集するために使い、クリックするとこの Agent に紐づくワークフローの編集画面が開きます。

> フロー編集の画面説明と操作については、[ワークフローの編集](bian-ji-gong-zuo-liu-cheng.md) を参照してください

## **会話ログ**

会話ログはこの Agent のすべての会話履歴を提供し、管理者はタイトル、ユーザー、会話時間範囲で履歴を絞り込めます。

ログには処理フローも保持されており、会話にエラーが発生したり性能が低かったりした場合、管理者は各返信が生成された処理フローを確認して原因を究明できます。

<figure><img src="../.gitbook/assets/image (199).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (200).png" alt=""><figcaption></figcaption></figure>

## **Web App**

Agent は次の図のように、質問応答サービスを提供するためにウェブページに埋め込むことができます：

<figure><img src="../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>

Agent をウェブページに埋め込んで使用したい場合は、この機能を使ってウェブページに埋め込むフロントエンドのコードを作成する必要があります。

### **AI WEBAPP の追加**

<figure><img src="../.gitbook/assets/image (207).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (208).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (209).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (210).png" alt=""><figcaption></figcaption></figure>

1. 「Agent 機能リスト」内の Web App に入ります
2. 「+」をクリックして _作成_ Web App ダイアログを開きます
3. 「名前」欄に名前を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-agent.md#duo-guo-yu-yan-she-ding) を参照してください
4. 「説明」欄に説明を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-agent.md#duo-guo-yu-yan-she-ding) を参照してください
5. 「保存」をクリックして完了します
6. 新しい Web App がリストに表示されます。「操作」メニューを使って「編集」、「有効期限の設定」、「削除」を行います
7. Web App 名をクリックして情報ページにアクセスし、「埋め込みコード」の確認、_アプリケーション言語_、_リクエストとトークンの制限_ などを設定します

> Note：各 Agent は複数の API キーと対応する埋め込みコードを持つことができ、異なる Web App インスタンスの有効期限や利用制限を個別に管理できます。

## API Key

API Key は本人確認のためのアクセスキーで、システムが Agent API を呼び出す際に、リクエストの送信元を識別し、対応する権限と利用クォータを適用できるようにします。API Key は外部に流出しないよう適切に保管してください。キーが漏洩した疑いがある場合は、ただちに交換し、そのキーを使用しているすべての連携設定を更新することをお勧めします。

<figure><img src="../.gitbook/assets/image (211).png" alt=""><figcaption></figcaption></figure>

### API Key の追加

<figure><img src="../.gitbook/assets/image (212).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (213).png" alt=""><figcaption></figcaption></figure>

1. 「Agent 機能リスト」内の API Key に入ります
2. 「+」をクリックして _作成_ API Key ダイアログを開きます
3. API Key の名前を入力します
4. Rate Limit を有効にするかどうかを選択し、数値を設定します
5. 「保存」ボタンをクリックします

> 注意： 保存後、ID と API キーをただちにコピーして、紛失しないようにしてください。

### Endpoint のコピー

Endpoint は Agent API のサービス入口の位置（URL）です。システムは対応する機能を実行するために、API リクエストをこの位置に送ります。利用シーンに応じて正しい Endpoint（例：テスト環境または本番環境）を選択し、リクエストを誤った環境に送ったり接続に失敗したりしないようにしてください。

Endpoint のコピーボタンは検索ボックスの横にあり、コピーボタンをクリックすると URL をコピーできます。URL をコピーする際は、どの環境にいるかに注意してください。

<figure><img src="../.gitbook/assets/image (214).png" alt=""><figcaption></figcaption></figure>
