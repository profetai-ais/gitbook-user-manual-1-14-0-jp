---
description: 「構成」モジュールは主にシステムの既定動作設定を管理するために使い、GPT の既定構成や default system prompt などの関連項目を含みます。
---

# 構成

## 翻訳

多言語翻訳やその他の関連翻訳の設定を制御します。

<figure><img src="../.gitbook/assets/image (412).png" alt=""><figcaption></figcaption></figure>

## **関連質問**

関連質問機能は、LLM がすでに返信した内容を使って関連質問を生成し、ユーザーがクリックするだけで質問応答を実行できるようにします。管理者は関連質問の生成設定を変更できます。

<figure><img src="../.gitbook/assets/image (274).png" alt=""><figcaption></figcaption></figure>

## タイトル生成

ユーザーの入力内容に基づいてタイトルを自動生成するために使います。システムはまず入力言語を識別し、次に簡潔でテーマ性のあるタイトルを生成します。

<figure><img src="../.gitbook/assets/image (275).png" alt=""><figcaption></figcaption></figure>

## **記憶設定**

### **記憶言語モデル**

画面右上のアバター内の Personalization 関連の内容に使用する言語モデルを設定するために使い、実際の利用シーンに応じて英語や中国語など適切な言語を選択できます。

<figure><img src="../.gitbook/assets/image (416).png" alt=""><figcaption></figcaption></figure>

### **記憶ベクトルモデル**

画面右上のアバター内の Personalization で、Memory の内容をベクトル化してデータベースに書き込む際に使用する embedding モデルを設定するために使います。

<figure><img src="../.gitbook/assets/image (415).png" alt=""><figcaption></figcaption></figure>

### ユーザー記憶ツール

AI がユーザーの記憶をどう判断、保存、更新、削除するかを設定するために使い、安全ルールに準拠した上で、長期的に使える好みや情報をシステムが保持するのを支援します。

<figure><img src="../.gitbook/assets/image (417).png" alt=""><figcaption></figcaption></figure>

### Agent 記憶の抽出

AI が会話から再利用可能なタスク実行の経験をどう抽出するかを設定するために使い、Agent が検証済みのフロー、ルール、操作方法を保持するのを支援します。

<figure><img src="../.gitbook/assets/image (418).png" alt=""><figcaption></figcaption></figure>

## 音声設定

ワークスペースで音声テキスト変換機能を使う際に必要な、変換のルールと制限条件のために使います。

<figure><img src="../.gitbook/assets/image (419).png" alt=""><figcaption></figcaption></figure>

## **スキルスキャン設定**

スキルをアップロードする際にスキャン機構を有効にするかどうかを制御するために使います。有効にすると、システムはスキルのアップロード時にスキャンを行います。無効にすると、アップロード時にスキャンを実行しません。

<figure><img src="../.gitbook/assets/image (420).png" alt=""><figcaption></figcaption></figure>

## 指示リライト設定

指示リライト設定では、ユーザーが入力した元の指示を、より明確で構造化され実行可能なプロンプトに自動的に整理できます。システムは原意を保ちつつ、曖昧で重複した内容を取り除き、必要な形式、口調、長さ、言語の制限を補い、複数ステップの要件を明確な行動指示に整理することで、後続のモデルがタスクをより正確に理解・実行できるようにします。

<figure><img src="../.gitbook/assets/image (421).png" alt=""><figcaption></figcaption></figure>

## Canvas 設定

**Canvas 設定**では、ユーザーの要件にキャンバス関連機能の有効化が必要かどうかを判断し、リクエスト内容に応じて適切な処理フローに自動的に振り分けます。要件が図表、フローチャート、関係図、インタラクティブ UI、ウェブアプリの説明に関わる場合、システムは優先的にキャンバス設計機能に処理を任せます。HTML 生成の要件が含まれる場合も、指定のフローを通じてコード編集機能に引き渡して実行します。要件が視覚化やウェブアプリの範囲に属さない場合は、通常の応答フローを維持し、不必要にキャンバス機能を有効化しないようにします。

<figure><img src="../.gitbook/assets/image (422).png" alt=""><figcaption></figcaption></figure>

## ログ分析

ログ分析は、AI がログを分析する際の判断方法と出力形式を設定するために使い、システムがエラー、トレンド、可用性、性能などの情報に基づいて全体の健全性を評価するのを支援します。

<figure><img src="../.gitbook/assets/image (423).png" alt=""><figcaption></figcaption></figure>

## AI Cron 設定

AI が自然言語のスケジュール記述を Spring CronExpression にどう変換するかを設定するために使い、ユーザーが使えるスケジュールルールを素早く生成するのを支援します。

<figure><img src="../.gitbook/assets/image (424).png" alt=""><figcaption></figcaption></figure>

## 既定モデル

モデル一覧内のモデルの並び順を設定するために使います。並び順はユーザーが呼び出せる権限に従って順に表示されます。

<figure><img src="../.gitbook/assets/image (425).png" alt=""><figcaption></figcaption></figure>
