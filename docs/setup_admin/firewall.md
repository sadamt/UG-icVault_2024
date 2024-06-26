---
title: ファイヤーウォール送受信の許可設定
---

サーバーのファイヤーウォール設定を確認します。

### Windows Defender ファイヤーウォール画面を開く

〔1〕Windows メニューから [コントロールパネル] を開きます。

![コントロールパネル](./img/firewall_001.png)

〔2〕コントロール パネルのメニューから [システムとセキュリティ] をクリックします。

![システムとセキュリティ](./img/firewall_002.png)

〔3〕[Windows Defenderファイアウォール] をクリックします。

![ファイヤーウォール](./img/firewall_003.png)

〔4〕左側メニュー欄の [詳細設定] をクリックします。

![詳細設定](./img/firewall_004.png)

〔5〕[セキュリティが強化されたWindows Defenderファイアウォール] の画面が開きます。

![ファイヤーウォール画面](./img/firewall_005.png)


### 受信の許可設定

〔1〕左側メニュー欄の [受信の規則] をクリックします。<br>
続いて、右メニュー [新しい規則] をクリックします。

![新しい規則](./img/firewall_006.png)

〔2〕[規則の種類] の設定では [ポート] を選択し、[次へ] をクリックします。

![ポート](./img/firewall_007.png)

〔3〕プロトコルおよびポートの設定では、[TCP] を選択し、[特定のローカル ポート] に[1433]を入力します。　
[次へ] をクリックします。

![プロトコルおよびポートの設定](./img/firewall_008.png)

〔4〕操作の設定では [接続を許可する] を選択し、[次へ] をクリックします。

![操作の設定](./img/firewall_009.png)

〔5〕プロファイルの設定では現在の接続設定の項目にチェックを入れ、[次へ] をクリックします。　
※不明の場合はすべての項目にチェックを入れます。

![プロファイルの設定](./img/firewall_010.png)


〔6〕名前の設定では、名前に [icVaultServerDataBase] を入力し、説明に [SQL Server(icVaultデータベースサーバ)] を入力します。

![名前の設定](./img/firewall_011.png)

[完了] をクリックします。

<p class="note">〔6〕の名前は上記以外の任意の名前でも問題ありません。サーバ管理者が分かりやすい名前を付けても大丈夫です。</p>


### 送信の許可設定

〔1〕左側メニュー欄の [送信の規則] をクリックします。<br>
続いて、右メニュー [新しい規則] をクリックします。

![新しい規則](./img/firewall_012.png)

〔2〕[規則の種類] の設定では [ポート] を選択し、[次へ] をクリックします。

![ポート](./img/firewall_007.png)

〔3〕プロトコルおよびポートの設定では、[TCP] を選択し、[特定のローカル ポート] に [1433] を入力します。　[次へ] をクリックします。

![プロトコルおよびポートの設定](./img/firewall_008.png)

〔4〕操作の設定では[接続を許可する]を選択し、[次へ] をクリックします。

![操作の設定](./img/firewall_009.png)

〔5〕プロファイルの設定では現在の接続設定の項目にチェックを入れ、[次へ] をクリックします。

![プロファイルの設定](./img/firewall_010.png)

※不明の場合はすべての項目にチェックを入れます。

〔6〕名前の設定では、名前に [icVaultServerDataBase] を入力し、説明に [SQL Server(icVaultデータベースサーバ)] を入力します。

![名前の設定](./img/firewall_011.png)

[完了] をクリックします。

<p class="note">〔6〕の名前は上記以外の任意の名前でも問題ありません。サーバ管理者が分かりやすい名前を付けても大丈夫です。</p>

以上で、外部との通信許可設定は完了です。
