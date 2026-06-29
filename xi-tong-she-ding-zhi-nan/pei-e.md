---
description: 管理者は使用クォータプランを作成・調整し、各ユーザーがシステムリソースを利用できる頻度と量を管理できます。
---

# クォータ

## クォータプラン

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="80">項目</th><th width="170">名前</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>名前</td><td>クォータプランの表示名（例：<code>default</code>, <code>VVIP</code>, <code>Plan VIP</code>）。</td></tr><tr><td>2</td><td>使用量リセット周期</td><td>クォータがリセットされる頻度（例：毎日、毎週、毎時）。</td></tr><tr><td>3</td><td>費用上限(USD)</td><td>各リセット周期内に許可される最大支出（米ドル換算）。<code>-1</code> は無制限を表します。</td></tr><tr><td>4</td><td>作成者</td><td>このプランを作成した管理者の名前。</td></tr><tr><td>5</td><td>変更日</td><td>クォータプランの変更時刻。</td></tr><tr><td>6</td><td>説明</td><td>クォータプランの用途に関する内部メモや説明。</td></tr><tr><td>7</td><td>操作</td><td>このプランを編集または削除するボタン。</td></tr></tbody></table>

## **クォータプランの追加**

管理者は、名前、説明、費用上限、リセット周期などのパラメータを設定して、新しい使用クォータプランを作成できます。これらのプランは、ここで設定した制限に従って、ユーザーが有料リソース（API token、モデル使用回数など）を消費する頻度を制御します。

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

1. システム設定 > 使用クォータ制限 に移動します。
2. Quota Plan タブを選択します。
3. プラスボタンをクリックして「クォータプランの追加/更新」フォームを開きます。
4. Name：プランの表示名。
5. Description：任意の内部メモ。
6. Cost Limit (USD)：各リセット周期に許可される金額（-1 は無制限）。
7. Usage Reset Cycle：毎日、毎週、毎時から選択します。
8. OK をクリックして新しいクォータプランを保存します。

## **既定のクォータプランの設定**

**既定のクォータプラン** は、特定のクォータプランを手動で割り当てない限り、新しく作成されるすべてのユーザーの基準となる使用制限を定義します。

<figure><img src="../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

1. Set Default Quota Plan タブに移動します。
2. Default User Quota Plan のドロップダウンメニューをクリックして、利用可能なプラン一覧を確認します。
3. 一覧から必要なプランを選択します（例：`既定`、`VVIP`、`超低クォータ`）。

> 注意：管理者は先に Quota Plan タブでプランを作成または更新してから、それを既定に設定できます。

## **クォータプランの紐づけ管理**

**クォータプランの紐づけ管理** 機能では、管理者が特定のユーザーに専用の使用クォータプランを手動で割り当て、既定の設定を上書きできます。

<figure><img src="../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

1. システム設定 > ユーザークォータプラン紐づけ管理 に移動します。
2. 「作成」をクリックして新しい紐づけを作成します。
3. 左側（Dataset）で割り当てるクォータプランを選択します（例：`既定`、`VVIP`、`Plan 1`）。
4. 右側（User）でドロップダウン一覧から1人または複数のユーザーを選択します。
5. 「+」ボタンをクリックして手動でユーザーを追加します。
6. OK をクリックして割り当てを確認します。

> 注意：一度割り当てると、その後に既定のプランを変更しても、そのユーザーは紐づけ済みのカスタムプランに従って実行されます。

## **クォータ調整記録**

**クォータ調整記録** ページは、ユーザーのクォータ使用量に対するすべての手動変更、特に **ユーザークォータプラン紐づけ管理** タブからの操作を記録します。

<figure><img src="../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

管理者が **ユーザークォータプラン紐づけ管理** タブで **更新アイコン** をクリックすると、システムはウィンドウを表示して **使用量リセットの理由** の入力を求めます。この欄は必須で、入力しないとリセット操作を完了できません。確認後、更新された予算と理由が「ユーザークォータ調整記録」ページに表示されます。

<figure><img src="../.gitbook/assets/image (8) (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="80">項目</th><th width="220">欄名</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>ユーザー名</td><td>クォータが手動で調整されたユーザーの名前。</td></tr><tr><td>2</td><td>処理前の予算 (USD)</td><td>調整前のユーザーの予算（米ドル換算）。</td></tr><tr><td>3</td><td>処理後の予算 (USD)</td><td>調整後の予算（米ドル換算）。</td></tr><tr><td>4</td><td>使用量リセットの理由</td><td>手動更新または修正の理由を記録するために使います。</td></tr><tr><td>5</td><td>作成日</td><td>調整を実行した日付。</td></tr></tbody></table>
