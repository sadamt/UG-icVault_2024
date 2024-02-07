---
title: 外部との通信許可設定
---

サーバーが外部との通信をできるよう設定してください。

### 外部との通信許可設定を確認

〔1〕スタートメニューから [icVault] → [icVaultServerMaintenanceTool] を起動します。

![icVaultServerMaintenanceTool](./img/network_settings_001.png)

〔2〕左メニューの [ツール] をクリックします。

![ツール](./img/network_settings_002.png)

〔3〕[構成マネージャ] をクリックします。

![構成マネージャ](./img/network_settings_003.png)

〔4〕[SQL Serverネットワークの構成] → [MSSQLSERVERのプロトコル] を選択します。TCP/IP の項目を右クリックし、[プロパティ] をクリックします。

![プロトコル](./img/network_settings_004.png)

〔5〕TCP/IP のプロパティが表示されます。
プロトコルのタブを選択し、[全般] → [すべて受信待ち]と[有効] が、<はい> に設定されていることを確認します。

![プロトコル](./img/network_settings_005.png)

〔6〕同じ画面の [IPアドレス] タブを選択し、現在使用している IPアドレス の項目をリストから探します。<br>
当該リストの [有効] の設定を、<はい> に設定し、[OK] をクリックします。

![IPアドレス](./img/network_settings_006.png)

〔7〕構成マネージャの画面に戻り、[SQL Serverのサービス] を選択します。<br>
SQL Server(MSSQLSERVER) の項目を右クリックし、[再起動] をクリックします。<br>
外部との通信が有効になります。

![SQL Serverのサービス](./img/network_settings_007.png)


以上で、外部との通信許可設定は完了です。
