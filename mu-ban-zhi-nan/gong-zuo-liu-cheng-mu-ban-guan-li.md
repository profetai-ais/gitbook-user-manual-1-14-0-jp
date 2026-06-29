# ワークフローテンプレート管理

## はじめに

フローテンプレートはワークフローアシスタントで使われ、ユーザーがワークフローアシスタントとの会話で入力したプロンプトをどう処理するかを、視覚的な方法で設計できるようにします。

> **注意**：既定では、AI Studio 管理者のみがこれらの設定を変更できます。

## **新しいワークフローテンプレートの作成**

> フローの編集操作については、[ワークフローの編集](../agent-zhi-nan/bian-ji-gong-zuo-liu-cheng.md) の説明を参照してください

## **新しいテンプレートの作成方法**

#### **新規テンプレート**

このオプションは空白のフローテンプレートを作成します。

<figure><img src="../.gitbook/assets/image (249).png" alt=""><figcaption></figcaption></figure>

1. 右上の「新規追加」ボタンをクリックします
2. 「名前」欄に名前を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-mu-ban-guan-li.md#duo-guo-yu-yan-she-ding) を参照してください
3. 「説明」欄に説明を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-mu-ban-guan-li.md#duo-guo-yu-yan-she-ding) を参照してください
4. 「確定」ボタンをクリックして追加を完了します。新しく作成したフローはテンプレート一覧に表示され、名前をクリックすると編集画面が開きます

#### 多言語設定

<figure><img src="../.gitbook/assets/image (250).png" alt=""><figcaption></figcaption></figure>

1. 画面の「地球」ボタンをクリックすると自動翻訳が行われます。ユーザーは内容を手動で編集することもできます
2. 自動翻訳が完了したら「確定」ボタンをクリックして内容を保存します

> 注意：「モデル」メニューの大規模言語モデルの選択肢は、実際のインストール環境の構成を基準としてください。説明文書に示された選択肢は参考用です。

#### **テンプレートから複製**

このオプションでは、既存のワークフローテンプレートを新しいフローに複製して編集できます。

<figure><img src="../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

1. テンプレート一覧から複製したいテンプレートを選択します
2. 複製ボタンをクリックします
3. 新しく作成したフローがテンプレート一覧に表示されます

#### **テンプレートのインポート**

このオプションでは、ファイルからワークフローテンプレートを新しいフローにインポートして編集できます。

<figure><img src="../.gitbook/assets/image (253).png" alt=""><figcaption></figcaption></figure>

1. 右上の「その他」ボタンをクリックし、「ファイルインポート」を選択します
2. 「ファイルアップロードエリア」をクリックしてインポートするテンプレートファイル（拡張子 `.pwflow` のファイル）を選択します
3. 「名前」欄に名前を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-mu-ban-guan-li.md#duo-guo-yu-yan-she-ding) を参照してください
4. 「説明」欄に説明を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](gong-zuo-liu-cheng-mu-ban-guan-li.md#duo-guo-yu-yan-she-ding) を参照してください
5. もう一度「確定」ボタンをクリックして追加を完了します。新しく作成したフローがテンプレート一覧に表示されます



## 権限

リスト権限については [モジュール権限ロールの紹介 - ワークフローテンプレートリスト権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#gong-zuo-liu-cheng-mu-ban-qing-dan) を参照してください。

権限設定については [権限操作機能の紹介 - Root 権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#root-quan-xian) を参照してください。

### ワークフローテンプレート権限

ロール権限については [モジュール権限ロールの紹介 - ワークフローテンプレート権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#gong-zuo-liu-cheng-mu-ban) を参照してください。

権限設定については [権限操作機能の紹介 - Object ロール権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#jue-se-quan-xian) を参照してください。
