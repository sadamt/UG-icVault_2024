---
title: インストール(アップデート)
---

# ソフトウェアのアップデート (サーバ)
本項目は、icVaultをご利用いただく際のシステム管理者向けのご案内になります。<br>
新しいバージョンのicVaultがリリースされた場合にアップデートを実施します。

**アップデートに必要なソフトウェア** 
<li>icVaultServerDataBase.msi</li>
<li>icVaultServerFileTransfer.msi</li>
<li>icVault.msi</li>  

<div class="note">
ユーザーの設定やアクセス権の設定は icVault に含まれます。<br>
データベースサーバもicVault.msl のアップデートを実施してください。。
</div>
<br>

## アップデートの手順

### 手順 1　インストールファイルを開く

インストールメディアを開きます。

![インストールメディア](./img/Install_re_001.png)


### 手順 2　icVaultServerDataBaseのアップデート

icVaultServerDataBase.msiをダブルクリックします。

![実行ファイル](./img/icVaultSDB_re_001.png)

1.　 セットアップウィザード画面が表示します。<br>
　　「次へ」をクリックします。

![セットアップウィザード](./img/icVaultSDB_001.png)

2.　インストールフォルダの選択<br>
　　※インストールフォルダはデフォルトを推奨します。<br>
　　「次へ」をクリックします。

![インストールフォルダの選択](./img/icVaultSDB_002.png)

3.　インストールの種類<br>
　　アップグレード インストールにチェックを入れ、「次へ」をクリックします。

![インストールの種類](./img/icVaultSDB_010.png)

4.　インストールの確認<br>
　　「次へ」をクリックします。

![インストールの確認](./img/icVaultSDB_004.png)

5.　インストールの実行<br>
　　数秒かかります
　　「次へ」をクリックします。

![実行](./img/icVaultSDB_005.png)

設定の復元が表示された場合は、選択してください。<br>
設定を引き継ぐ場合は〔はい〕<br>
設定を引き継がない場合は〔いいえ〕をクリックします。<br>

![設定の復元](./img/icVaultSDB_011.png)

<div class="note">
〔いいえ〕をクリックし、設定を引き継がなかった場合は、ユーザがicVault使用時にファイル一覧がクリアされた状態になります。
</div>
<br>

6.　データベースのアップデート<br>
　　データベースの作成/アップデートは自動で開始されます。<br>
　　※数秒かかる場合があります。

![データベースのアップデート](./img/icVaultSDB_007.png)

7.　アップデートの完了<br>
　　「閉じる」をクリックし、完了します。

![アップデートの完了](./img/icVaultSDB_009.png)


### 手順 3 icVaultServerFileTranserのアップデート
icVaultServerDataBase.msiをダブルクリックします。

![トランスファーファイル](./img/Trans_install_re_001.png)

1.　セットアップウィザード画面が表示します。<br>
　　修復へチェックを入れ、「完了」をクリックします。

![セットアップウィザード](./img/Trans_install_re_002.png)

2.　インストールが開始されます。<br>
　　設定の復元確認メッセージが表示されます。<br>

![復元のインストール](./img/Trans_install_re_003.png)

　　続いて、〔OK〕をクリックします。

![復元確認](./img/Trans_install_re_004.png)

<div class="note">
〔いいえ〕をクリックし、設定を引き継がなかった場合は、ユーザがicVault使用時にファイル一覧がクリアされた状態になります。
</div>
<br>

3.　アップデートの完了<br>
　　「閉じる」をクリックし、完了します。

![アップデート完了](./img/Trans_install_re_005.png)


### 手順 4 icVaultのアップデート
icVault.msiをダブルクリックします。<br>
※ユーザーアカウント制御画面が表示された場合は「はい」をクリックします。

![クライアントファイル](./img/icVault_install_re_001.png)

1.　セットアップウィザード画面が表示されます。<br>
　　「次へ」をクリックします。

![インストールメディアマウント](./img/Cli/Client_wizard.png)

2.　インストールフォルダの選択<br>
　　インストール先とユーザー条件を指定します。<br>
　　前回と同じ階層を確認し、「次へ」をクリックします。

![インストールメディアマウント](./img/Cli/Client_wizard_2.png)

3.　インストール開始<br>
　　※数秒かかる場合があります。

![インストールメディアマウント](./img/Cli/Client_wizard_4.png)

4.　インストールの完了<br>
　　「閉じる」をクリックし、終了します。

![インストールメディアマウント](./img/Cli/Client_wizard_5.png)
