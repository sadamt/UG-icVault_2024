---
title: ファイルの取得
---

# icVault からファイルを取得する
本項目では icVault に登録されているデータを自身のPCに取得(保存)する手順を説明します。<br>
icVault では、設計データを登録していても各設計者が同じデータを自身の PC に保管しておくこともできます。<br>
そのため、複数の設計者が同じデータを作成・編集する場合はどれが最新データか分からなくなる場合があります。<br>
<br>
icVault をご活用いただくことで、常に登録された最新バージョンのデータを最新状態として管理・運用することができます。<br>
また自身が設計していないが、隣接関係のデータを参照として取得することも可能です。
参照で取得したデータは、チェックインできないため、誤って変更を登録(チェックイン)してしまう操作を防ぐことができます。


![ファイル一覧‗取得](./img/FileGet_001.png)

<table>
<tr>
<th>データを取得</th>
<td>ファイル一覧で選択したファイルのみ取得します。</td>
</tr>
<tr>
<th>外部リンクも含めてデータ取得</th>
<td>ファイル一覧で選択したファイルと外部リンクで紐づいているファイルを取得します。</td>
</tr>
<tr>
<th>現在のシーンにインポート</th>
<td>チェック有り：<br>
　開いているシーンファイルに読み込まれます。<br>
<br>
チェック無し：<br>
　新しいシーンファイルで開きます。 
</td>
</tr>
<tr>
<th>IRONCAD Sceneファイル も取得</th>
<td>3D と紐づいている 2Dファイル(exb) を選択した場合に選択できます。<br>
　チェック有り：<br>
　　3Dファイル も一緒に取得します。<br>
<br>
　チェック無し：<br>
　　選択した 2Dファイル のみ取得します。
</td>
</tr>
</table>

### データを取得する場合
※先に [現在のシーンにインポート]設定 を選択してください。<br>

一覧からファイルを選択し、[データを取得] をクリックします。


### 外部リンクも含めてデータ取得する場合
※先に [現在のシーンにインポート]設定 を選択してください。<br>

1. 一覧からファイルを選択し、[外部リンクも含めてデータ取得] をクリックします。

2. 取得する条件を設定

![外部リンク含めて取得画面](./img/FileGet_002.png)

<table>
<tr>
<th>新しい部品</th>
<td>icVault に登録されているデータとは別に新しいデータとして取得します。</td>
</tr>
<tr>
<th>チェックアウト</th>
<td>データ取得と同時にチェックアウトします。</td>
</tr>
<tr>
<th>参照に設定</th>
<td>参照データとして取得します。　※チェックインできません。
</td>
</tr>
</table>

<div class="note">
<ul>
参照として取得したデータは通常の IRONCAD と同じデータで編集も可能です。<br>
ローカル作業時は編集状態を保存することも可能ですが、チェックインが出来ない設定となっているため
チェックイン操作の際に警告メッセージが表示されます。
</ul>
</div>

　3. 外部リンクファイルの選択　※必要時のみ<br>

外部リンクされたファイルは、IRONCAD と同じくアイコンに外部リンクのマークが付きます。<br>
外部リンクファイルは別のバージョンを取得したい場合は、画面右上の [バージョン選択画面を表示] にチェックを入れます。

![外部リンク含めて取得画面](./img/FileGet_003.png)

バージョン一覧から選択し、[反映] をクリックします。

ただし古いバージョンを反映させた場合、チェックアウトはできません。

![外部リンク含めて取得画面](./img/FileGet_004.png)

　4. データを取得する<br>

設定完了後、右下の [決定] をクリックします。<br>
続いて、保存するフォルダを指定し [保存] します。
