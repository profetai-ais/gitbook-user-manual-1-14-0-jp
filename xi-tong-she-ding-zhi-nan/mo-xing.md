---
description: >-
  AI Studio では、IT 担当者が ChatGPT や Gemini などの外部で購読する大規模言語モデル（LLM）サービスを連携したり、自社の計算資源上にデプロイしたオンプレミスの大規模言語モデルとの接続を設定したりできます。
---

# モデル

## **大規模言語モデルの追加**

<figure><img src="../.gitbook/assets/image (270).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (271).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (272).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (273).png" alt=""><figcaption></figcaption></figure>

1. 入った後、右上の「＋新規追加」をクリックして設定を開始します。
2. サービスプロバイダーを選択します（例：OpenAI / Azure / Gemini / Ollama / Claude）
3. プロバイダーごとに内容を設定します
   1. 名前：カスタマイズでき、システム内に表示されるモデル名になります
   2.  モデル：使用するモデルを入力してください

       > 注意：手動で記入してください。システムは選択肢を自動的に列挙しません。（例：`gpt-5`、`gpt-4o`、`gemini-pro`、`llama3-70b` …など）
       >
       > 例えば誤って `gpt-6` と入力した場合、Agent のテスト時に次のエラーメッセージが表示されます：
       >
       > Received Model Group=gpt-6
       >
       > Available Model Group Fallbacks=None
       >
       > モード：モデルを自分で入力する場合は、別途モードを選択する必要があります（例：Chat / Embedding）
   3.  API ベース：プロバイダーが提供する API Key を入力してください

       > 注意：誤って入力すると、システムは認証エラーを返します
       >
       > * OpenAI：API のプレフィックス（Prefix）を記入するだけで構いません。例：`https://api.openai.com/v1`
       > * Gemini：API Base URL を記入する必要はなく、システムが自動的にルーティングを処理します。
   4. API Key：API Key を記入してください
   5. 組織：必須ではありません。通常のキーは空欄で構いませんが、一部の OpenAI で短いキーを使用する場合は記入が必要なことがあります。
4. 詳細設定
   1. **クラウドモデル** を使用する場合 → 空欄のままにし、システムが自動的に最新価格を更新するようにすることをお勧めします。
   2. **自社デプロイモデル** を使用する場合 → 料金を自分で記入するか検討できます。
5. 「作成」をクリックして設定を完了します。

### よくある質問：モデルの Logo が実際に接続するプロバイダーと一致しない

<figure><img src="../.gitbook/assets/image (304).png" alt="" width="561"><figcaption></figcaption></figure>

モデル管理ページでは、モデルの Logo はモデル作成時に選択したプロバイダー（Provider）に基づいて表示されます。

例：モデル作成時に選択したプロバイダーが OpenAI の場合、画面には GPT / OpenAI 関連の Logo が表示されます。Azure OpenAI を選択した場合は、Azure 関連の表示になります。

そのモデルが実際に接続しているのは Azure API でも、モデル作成時のプロバイダー欄で OpenAI を選択していると、「実際は Azure API を使用しているが画面には GPT の Logo が表示される」という状況が起こることがあります。

これはモデル作成時のプロバイダー選択と画面表示ロジックの差異によるもので、モデルは設定済みの API URL、Key、関連パラメータに従って呼び出されます。モデルが接続テストと使用を正常に完了できれば、現在の API 接続が正常に動作していることを意味します。

画面の Logo を実際のプロバイダーと一致させる必要がある場合は、モデルを追加または再作成する際に、プロバイダー欄で正しいサービスソースを選択していることを確認することをお勧めします。

### **モデル設定内容の説明**

<table><thead><tr><th width="186">設定項目</th><th width="288">説明</th><th>選択肢</th></tr></thead><tbody><tr><td>サービス名</td><td>モデルを提供するサービス名</td><td><code>openai</code>, <code>gemini</code>, <code>ollama</code> (on-premises)</td></tr><tr><td>モード</td><td>モデルの種類</td><td><code>chat</code>, <code>embedding</code></td></tr><tr><td>モデル</td><td>サービスが提供する使用可能なモデル</td><td>例：<code>gpt-4.1</code>, <code>gemini-2.0-flash</code> など、システムインストール時の設定による</td></tr><tr><td>名前</td><td>AI Studio でこのモデルを識別するために使う名前</td><td>既定ではモデルと同じ。ユーザーが入力</td></tr><tr><td>説明</td><td>モデルの説明</td><td>ユーザーが入力</td></tr><tr><td>API キー/API ベース</td><td>サービスで <code>openai</code> と <code>gemini</code> を選択したときはキーを入力し、<code>ollama</code> を選択したときはモデル API サービスの URL を入力します</td><td>ユーザーが入力</td></tr><tr><td>カスタム価格（詳細設定）</td><td>モデルサービスの価格を提供するかどうか。生成 AI 利用のコスト計算に使います</td><td>ユーザーの選択</td></tr><tr><td>価格設定モデル（詳細設定）</td><td>サービスをどう価格設定するか</td><td>既定は100万トークンあたり</td></tr><tr><td>入力コスト（詳細設定）</td><td>金額の数値を入力</td><td>ユーザーが入力</td></tr><tr><td>出力コスト（詳細設定）</td><td>金額の数値を入力</td><td>ユーザーが入力</td></tr><tr><td>有効状態</td><td>モデルの有効化／停止</td><td>ユーザーの選択</td></tr></tbody></table>

> 注意：モデルの作成完了後は、サービス名、モード、モデルを変更できません。

### モデルサポート一覧

AI Studio は現在、以下を含む複数のモデル接続ソースをサポートしています：

* OpenAI
* Azure OpenAI
* Google / Gemini
* Ollama
* Anthropic Claude
* AWS Bedrock
* Google Vertex AI
* DeepSeek
* Mistral AI
* Cohere
* OpenRouter
* NVIDIA NIM
* GLM
* MiniMax
* Qwen

> 注意：上記の一覧は主に AI Studio が現在サポートするモデル接続ソースです。実際の利用時、モデルは Cloud または On-premise の方式でデプロイでき、顧客の環境ニーズ、モデルライセンス、API サービス、オンプレミス化デプロイの条件によって異なります。

## 権限

{% hint style="info" %}
モデルモジュールは AI Studio 管理者のみがアクセスできるため、リスト権限の設定はありません。

AI Studio のロール権限については [AI Studio のロールと権限の説明](../ru-men-zhi-nan/ai-studio-jue-se-yu-quan-xian-shuo-ming.md) を参照してください。
{% endhint %}

### モデル権限

ロール権限については [モジュール権限ロールの紹介 - モデル権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#mo-xing) を参照してください。

権限設定については [権限操作機能の紹介 - Object ロール権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#jue-se-quan-xian) を参照してください。
