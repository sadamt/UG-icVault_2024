---
title: ファイルの削除
---

# ファイルの削除
ユーザが icVaultSmartGateway のファイル削除(ごみ箱)、バージョンを削除(ごみ箱)を実行し、
さらにごみ箱から完全に削除されたファイルが表示されます。<br>
<br>
ユーザが icVaultアドイン でごみ箱に移動した時点では、サーバにデータが残っています。<br>
管理者は、ごみ箱に移動された全データもしくはバージョン毎にサーバから完全に削除することが可能です。<br>

![ファイル削除画面](./img/File_remove_001.png)

<div class="note">
<ul>
不要なデータは定期的にサーバから完全に削除されることを推奨します。
</ul>
</div>
<br>

<div class="caution">
<ul>
削除後は元に戻せませんのでご注意ください。
</ul>
</div>
<br>

### 1. 削除するバージョンを選択する
ファイルの削除(全バージョン)または(特定のバージョン)のリクエスト一覧から、ファイルを選択します。

![ファイルの選択](./img/File_remove_002.png)

### 2. 処理方法を選択する
選択したファイルに対し、適用する処理を選択します。

![各種ボタンの説明](./img/File_remove_003.png)

<table>
<tr>
<th>ファイルをダウンロード</th>
<td>icVaultアドインから削除したファイルをダウンロードします。</td>
</tr>
<tr>
<th>Vaultに復元</th>
<td>icVaultアドイン (ユーザ側)へデータを復元します。<br>
※復元オプション:復元する場所を事前にチェックします。
</td>
</tr>
<tr>
<th>システムから完全削除</th>
<td>ファイルサーバから完全にファイルを削除します。</td>
</tr>
</table>

#### ファイルをダウンロードする場合
保存場所を指定して、[開く] をクリックします。

#### Vaultに復元する場合
ファイルの復元の確認メッセージが表示されます。<br>
[はい] をクリックします。

![復元](./img/File_remove_004.png)

#### システムから完全削除する場合
ファイルから完全に削除の確認メッセージが表示されます。<br>
[はい] をクリックします。

![完全削除](./img/File_remove_005.png)
