# ナレッジベースの管理

## はじめに

> 注意：既定では、AI Studio 管理者、AI Studio コラボレーター、ナレッジベース管理者、ナレッジベースコラボレーター、ナレッジベースメンバーのみがナレッジベース機能を利用できます。ナレッジベースを利用できない場合は、管理者に権限を確認してください。

ナレッジ内のデータセットの整理方法は下図のとおりです：

<figure><img src="../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>

## **新しいナレッジの作成**

### **手動でナレッジを作成する**

<figure><img src="../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

1. 左側メニューの「ナレッジベース」項目をクリックします
2. 画面右上の「+」ボタンをクリックします
3. 「名前」欄に名前を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](guan-li-zhi-shi-ku.md#duo-guo-yu-yan-she-ding) を参照してください
4. 「説明」欄に説明を入力した後、右側のボタンをクリックして多言語ラベルを作成します。[多言語設定](guan-li-zhi-shi-ku.md#duo-guo-yu-yan-she-ding) を参照してください
5. 「インデックスモデル」メニューをクリックして、このナレッジがテキストを意味ベクトルに変換する際に使用するモデルを選択します
6. 「保存」ボタンをクリックして追加を完了します

### 多言語設定

<figure><img src="../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

1. 画面の「地球」ボタンをクリックすると自動翻訳が行われます。ユーザーは内容を手動で編集することもできます
2. 自動翻訳が完了したら「保存」ボタンをクリックして内容を保存します

### **ナレッジのインポート**

<figure><img src="../.gitbook/assets/image (387).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (389).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (390).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (391).png" alt=""><figcaption></figcaption></figure>

1. ナレッジベースタブに移動します
2. 右上の「その他」ボタンをクリックし、「ファイルインポート」を選択します
3. 埋め込みモデルを選択した後、テストボタンをクリックしてモデルが正常に使用できるかテストします
   1. これはナレッジベースのインデックスを作成するためのモデルです。ナレッジをインポートした後、システムはこのモデルを使ってナレッジベースの内容を再インデックスし、以降の検索や Agent の回答時に使用します
4. テストに成功すると、システムは成功メッセージを表示します。テストに失敗した場合は、他の利用可能なモデルを選び直すか、そのモデルが正しく設定されているか、利用権限があるか、モデルサービスが正常に接続できるかを確認してください。確認後、閉じるボタンをクリックしてウィンドウを閉じます
5. インポートするファイルを選択します
6. インポートボタンをクリックしてインポートを完了します

> 注意： 先にモデルをテストし、テストに成功してから次のインポート操作に進む必要があります。

## 権限

リスト権限については [モジュール権限ロールの紹介 - ナレッジベースリスト権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#zhi-shi-ku-qing-dan) を参照してください。

権限設定については [権限操作機能の紹介 - Root 権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#root-quan-xian) を参照してください。

### ナレッジ権限

ロール権限については [モジュール権限ロールの紹介 - ナレッジ権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#zhi-shi) を参照してください。

権限設定については [権限操作機能の紹介 - Object ロール権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#jue-se-quan-xian) を参照してください。

### データセット権限

ロール権限については [モジュール権限ロールの紹介 - データセット権限](../ru-men-zhi-nan/quan-xian-gong-neng-jie-shao.md#shu-ju-ji) を参照してください。

権限設定については [権限操作機能の紹介 - Object アクセス権限](../ru-men-zhi-nan/quan-xian-cao-zuo-gong-neng-jie-shao.md#cun-qu-quan-xian) を参照してください。
