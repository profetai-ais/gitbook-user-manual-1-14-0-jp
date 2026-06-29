---
description: 作業管理は、Agent が実行中の各作業（Jobs）を集中管理・追跡し、各作業の状態、責任の所在、進捗の変化を明確に把握するために使います。
---

# 作業管理

## はじめに

<figure><img src="../.gitbook/assets/image (215).png" alt=""><figcaption></figcaption></figure>

ユーザーが要件を提出すると、システムはそれを実行可能な作業項目に分解し、Job Manager で対応する Task を作成します。各 Task には、明確な Job、説明、現在の状態（例：待機中、進行中、完了、失敗／要対応）、作成・更新日時、関連する入力と成果物、必要な実行記録が含まれ、ユーザーが遡って照合しやすくなっています。

## タスク状態の紹介

状態（Status）は全部で8種類あります：

<table><thead><tr><th width="224">状態名</th><th>説明</th></tr></thead><tbody><tr><td>PENDING</td><td>作成済みで、キューへの投入待ち／未派送</td></tr><tr><td>QUEUED</td><td>キュー内で実行を待機中</td></tr><tr><td>RUNNING</td><td>実行中</td></tr><tr><td>SUCCEEDED</td><td>正常に完了</td></tr><tr><td>FAILED</td><td>実行失敗</td></tr><tr><td>STOPPED</td><td>停止された（中止）</td></tr><tr><td>CANCELED</td><td>キャンセルされた</td></tr><tr><td>PAUSED</td><td>一時停止中</td></tr></tbody></table>

## Job ページの説明

確認したい Task 名をクリックすると、ポップアップウィンドウが開き、その下の Job を閲覧できます。

<figure><img src="../.gitbook/assets/image (216).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (217).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="101">項目</th><th width="177">名前</th><th>説明</th></tr></thead><tbody><tr><td>1</td><td>やり直し</td><td>Job を再実行します</td></tr><tr><td>2</td><td>続行</td><td>Job の作業進捗を続行します</td></tr><tr><td>3</td><td>詳細情報</td><td>詳細情報を確認します</td></tr><tr><td>4</td><td>一時停止</td><td>Job の作業進捗を一時停止します</td></tr><tr><td>3</td><td>キャンセル</td><td>この Job の作業タスクをキャンセルします</td></tr></tbody></table>
