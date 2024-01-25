---
title: インストール(新規)
---

# ソフトウェアのインストール (サーバ)
本項目は、icVaultをご利用いただく際のシステム管理者向けのご案内になります。<br>

**インストールするソフトウェア** 
<li>1_icVaultServerDataBase_NewInstall.cmd　※初回のみ</li>
<li>icVaultServerDataBase.msi</li>
<li>icVaultServerFileTransfer.msi</li>
<li>icVault.msi</li> 

<div class="note">
<ul>
ユーザーの設定やアクセス権の設定はクライアント側でインストールするicVault.msi に含まれます。<br>
データベースサーバーにもicVault.msi をインストールすることをお勧めします。
</ul>
</div>


## icVaultサーバーの推奨システム条件
<table>
<tr>
<th>CPU</th>
<td>2 コア以上(2.5GHz以上)<br>
</td>
</tr>
<tr>
<th>RAM(メモリ) </th>
<td>8GB以上<br>
</td>
</tr>
<tr>
<th>ハードディスク容量</th>
<td>200GB以上<br>
</td>
</tr>
<tr>
<th>OS</th>
<td>Windows Server 2019 Standard/ Essentioas/ IoT Strage</td>
</tr>
<tr>
<th>SQL </th>
<td>Microsoft SQL Server 2019 Standard/ Express</td>
</tr>
</table>

<div class="note">
<ul>
<li>Windows Server の種類によってはアクセスするユーザー分のCALが別途必要です。</li>
<li>余程のユーザー数や大量のデータを取り扱わない限りExpressで運用可能です。</li>
</ul>
</div>

## インストールの手順

### 手順 1　インストールファイルを開く

1.　インストールメディアを開きます。

![インストールメディアマウント](./img/Install_001.png)

<div class="caution">
<ul>
インストールファイル一式をローカルフォルダへ移動して作業をする場合は、保存階層のパスの長さにご注意ください。
Windows10 のパス長さには制限があります。<br>
 256文字を超えるパスの場合、インストールが正常に終了しません。<br>
フォルダに日本語を使用している場合 子音のパスは2とカウントされます。<br>
例) は → ha
</ul>
</div>

2.　icVaultServerDataBaseを開き、1_icVaultServerDataBase_NewInstall.cmd をダブルクリックします。

![icVSDBフォルダ](./img/icVaultSDB_120.png)

インストールが開始されます。3 つのソフトウェアがインストールされます。

<table>
<tr>
<th>SQL Server 2019 Express</th>
<td>icVaultのデータベース本体<br>
(自動インストール)
</td>
</tr>
<tr>
<th>SQL Server Management Studio </th>
<td>データベースを操作するツール<br>
(自動インストール)
</td>
</tr>
<tr>
<th>icVaultServerDataBase</th>
<td>データベースの作成・アップデートするツール<br>
(手動でインストールが必要)
</td>
</table>

### 手順 2　データベースのインストール

初めに自動でインストールが開始されます。

#### 1. SQL Server 2019のインストール [自動]

※インストールには数分かかる場合があります。
![SQLServerDataBaseインストール開始画面](./img/SQL_Server2019.png)
![SQLServerDataBaseインストールメッセージ](./img/SQL_Server2019_2.png)
![セットアップfileのインストール](./img/SQL_Server2019_3.png)
![インストールの進行状況](./img/SQL_Server2019_4.png)

インストール完了後、「次へ」をクリックします。


#### 2. SQL Server Management Studioのインストール [1に続き自動でインストールが開始されます] 
※インストールには数分かかる場合があります。
![インストール①](./img/SQL_ServerManage_Studio.png)
![インストール②](./img/SQL_ServerManage_Studio_2.png)

#### 3. icVaultServerDataBaseのインストール [手動]

SQL Server Management Studioのインストールが終了後に自動でセットアップウィザードが表示されます。<br>

※自動でセットアップウィザードが表示されない場合は、以下をダブルクリックしてください。

![icVSDBフォルダ](./img/icVaultSDB_000.png)

1.　セットアップウィザード画面が表示します。<br>
　　「次へ」をクリックします。

![セットアップウィザード](./img/icVaultSDB_001.png)

2.　インストールフォルダの選択<br>
　　インストール先とユーザー条件を指定します。<br>
　　※インストールフォルダはデフォルトを推奨します。<br>
　　「次へ」をクリックします。

![インストールフォルダの選択](./img/icVaultSDB_002.png)

3.　インストールの種類<br>
　　新規インストールにチェックを入れます。<br>
　　〔次へ〕をクリックします。

![インストールの種類](./img/icVaultSDB_003.png)

4.　インストールの確認<br>
　　〔次へ〕をクリックします。

![インストールの確認](./img/icVaultSDB_004.png)

5.　データベースのインストール<br>
　　※インストールには数分かかる場合があります。

![インストール開始](./img/icVaultSDB_005.png)
![データベースのインストール](./img/icVaultSDB_006.png)<br>

(データベースのアップデートを開始します。)
![データベースのアップデート](./img/icVaultSDB_007.png)<br>
(データベースのアップデート完了)
![データベースのアップデート完了](./img/icVaultSDB_008.png)

※完了後、ウィンドウは自動で閉じます。

6.　インストールの完了<br>
　　「閉じる」をクリックし、終了します。

![インストール完了](./img/icVaultSDB_009.png)

#### インストール後の確認
Windowsのスタートメニューに以下の3つのフォルダが追加されていることを確認します。

<li>icVault</li>
<li>Microsoft SQL Server2019</li>
<li>Microsoft SQL Server Tools 18</li>

![スタートメニュー](./img/Startmenu_001.png)


### 手順 3　icVaultServerFileTranserのインストール

icVaultServerFileTransferを開き、icVaultServerFileTransfer.msiをダブルクリックします。

![インストールメディア](./img/icVSFileTrans.png)

1.　セットアップウィザード画面が表示します。<br>
　　「次へ」をクリックします。

![Transインストールウィザード](./img/Trans_wizard.png)

2.　インストールフォルダの選択 <br>
　　インストール先とユーザー条件を指定します。<br>
　　※インストールフォルダはデフォルトを推奨します。<br>
　　「次へ」をクリックします。

![Transインストールウィザード](./img/Trans_folder_select.png)

3.　インストールの確認<br>
　　「次へ」をクリックします。<br>
　　※数秒かかります。

![Transインストールウィザード](./img/Trans_install_confirm.png)

4.　データベースのインストール [自動でインストールが開始されます。<br>
　　※インストールには数分かかる場合があります。

![Transインストールウィザード](./img/Trans_install.png)

5.　icVaultで使用する全データの保存場所を指定します。<br>
　　・指定しない場合は「OK」をクリックします。<br>
　　・保存場所を指定する場合は「参照」をクリックします。

![Transインストールウィザード](./img/Trans_pass.png)

5-1.　指定せず「OK」をクリックした場合は以下のメッセージが出ます。<br>
　　「はい」をクリックします。　※自動的にC:\icVaultに設定されます。

![Transインストールウィザード](./img/Trans_pass_ok.png)

5-2.　保存場所を指定する場合は「参照」をクリックし、保存場所を選択後に「開く」をクリックします。

![Transインストールウィザード](./img/Trans_pass_sitei.png)

　　「OK」をクリックします。

![Transインストールウィザード](./img/Trans_pass_sitei_2.png)

6.　インストールの完了<br>
　　「閉じる」をクリックし、終了します。

![Transインストールウィザード](./img/Trans_pass_sitei_3.png)

#### インストール後の確認

タスクマネージャーを起動し、サービスにicVaultFileTransferServerが追加され{実行中}になっていることを確認します。

![Transインストールウィザード](./img/Trans_kakunin.png)


### 手順 4　icVaultのインストール(クライアントと同じ)
icVaultを開き、icVault.msiをダブルクリックします。

![Transインストールウィザード](./img/Cli/Install_media_2.png)

1.　セットアップウィザード画面が表示します。<br>
　　「次へ」をクリックします。

![icVaultウィザード](./img/Cli/Client_wizard.png)

2.　インストールフォルダの選択 <br>
　　インストール先とユーザー条件を指定します。<br>
　　※インストールフォルダはデフォルトを推奨します。<br>
　　「次へ」をクリックします。

![icVaultフォルダ指定](./img/Cli/Client_wizard_2.png)

3.　インストールの確認<br>
　　「次へ」をクリックします。<br>
　　※数秒かかります。

![icVault確認](./img/Cli/Client_wizard_3.png)

4.　icVaultのインストール [自動でインストールが開始されます]<br>
　　※インストールには数分かかる場合があります。

![icVaultインストール](./img/Cli/Client_wizard_4.png)

5.　インストールの完了<br>
　　「閉じる」をクリックし、終了します。

![インストール完了](./img/Cli/Client_wizard_5.png)


#### インストール後の確認
Windowsのスタートメニューに以下の3つのファイルが追加されていることを確認します。

![スタートメニューの確認](./img/Cli/icVault_install_naiyou.png)
