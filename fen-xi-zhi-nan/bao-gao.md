---
description: 分析 は、レポートやデータ分析結果を確認するためのページです。ユーザーはこのページで図表、レポート、関連する分析内容を確認し、データの状況を素早く把握して、閲覧と読み取りの効率を高められます。
---

# レポート

## はじめに

レポートは AI Studio の利用状況と運用分析レポートを提供し、管理者がプラットフォーム内の Token、Quota、タスク実行、機能利用状況を追跡するのを支援します。ユーザーは視覚化ダッシュボードで Session、Memory、Workflow、RAG、Speech などの関連データを確認でき、コスト分析、使用量の追跡、運用管理の参考にできます。

このページはレポートとデータ視覚化ツールを統合しており、ユーザーは権限に応じて作成済みの Dashboard、Chart、Dataset を確認できます。

<figure><img src="../.gitbook/assets/image (401).png" alt=""><figcaption></figcaption></figure>

## Dashboard

**Dashboard** は、作成済みの分析ダッシュボードを集中的に表示するために使います。各 Dashboard は1つ以上の図表を含み、特定テーマのデータ状況を観察するために使います。

一般的な Dashboard には以下の分析テーマが含まれます：

* Agent の利用状況
* Token の使用量とコスト
* ユーザー活動の分析
* Knowledge Base と Agent の関連
* 権限とアクセス状況
* タスク実行と異常監視

Dashboard 一覧では、ユーザーは名前、状態、オーナー、最終更新日時を確認できます。Dashboard 名をクリックすると、その Dashboard に入って詳細な図表内容を確認できます。

## Chart

**Chart** は、レポートの図表を管理または作成するために使います。図表を作成する際、ユーザーはまずデータセットを選択し、次に図表の種類を選択する必要があります。

システムは以下のような複数の図表タイプをサポートします：

* Area Chart
* Bar Chart
* Big Number
* Line Chart
* Pie Chart
* Table
* Heatmap
* Pivot Table
* Scatter Plot
* Treemap

図表タイプによって適したデータが異なります。例えば、トレンドデータは Line Chart、比率データは Pie Chart、明細データは Table、重要な数値は Big Number が使えます。

Chart を作成する機能は通常、レポート管理権限を持つユーザーに提供されます。一般ユーザーは権限に応じて既存の図表や Dashboard を確認できます。

## Dataset

**Dataset** は、図表や Dashboard の作成に使えるデータセットを表示します。Dataset はレポート分析のデータソースで、図表は選択した Dataset 内の欄やデータ内容に基づいて生成されます。

Dataset 一覧では、ユーザーはデータセット名、タイプ、データベース、Schema、オーナー、最終更新日時を確認できます。

## 注意事項

Report で確認できる Dashboard、Chart、Dataset はユーザーの権限によって異なります。特定のレポートやデータセットが表示されない場合は、対応する閲覧または管理の権限を備えているか確認してください。

このページは主にデータの確認と分析に使います。Dashboard、Chart、Dataset を調整する必要がある場合は、レポート管理権限を備えているか確認し、実際のニーズに応じて設定してください。
