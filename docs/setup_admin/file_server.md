---
title: ファイルサーバの送受信の許可設定
---

ファイルサーバーの通信許可設定を実施します。

### Windows Defender ファイヤーウォール画面を開く

〔1〕Windows メニューから [コントロールパネル] を開きます。

![コントロールパネル](./img/file_server_001.png)

〔2〕コントロール パネルのメニューから [システムとセキュリティ] をクリックします。

![システムとセキュリティ](./img/file_server_002.png)

〔3〕[Windows Defenderファイアウォール] をクリックします。

![ファイヤーウォール](./img/file_server_003.png)

〔4〕左側メニュー欄の [詳細設定] をクリックします。

![詳細設定](./img/file_server_004.png)

〔5〕[セキュリティが強化されたWindows Defenderファイアウォール] の画面が開きます。

![ファイヤーウォール画面](./img/file_server_005.png)


### 受信の許可設定

〔1〕左側メニュー欄の [受信の規則] をクリックします。<br>
続いて、右メニュー [新しい規則] をクリックします。

![新しい規則](./img/file_server_006.png)

〔2〕[規則の種類] の設定では [プログラム] を選択し、[次へ] をクリックします。

![プログラム](./img/file_server_007.png)

〔3〕[このプログラムのパス(T):] にチェックし、[参照] をクリックします。

![プロトコルおよびポートの設定](./img/file_server_008.png)

〔4〕icVaultServerFileTransfer のインストールパスに移動し、icVault FileTransfer Server.exe を選択し、[開く] をクリックします。<br>
※標準では C:\Program Files\CreativeMachine\icVaultServerFileTransfer にインストールされています

![操作の設定](./img/file_server_009.png)

〔5〕選択したパスが表示されたことを確認し、[次へ] をクリックします。

![プログラムの参照先設定](./img/file_server_010.png)

〔6〕[接続を許可する(A)] にチェックを入れ、[次へ] をクリックします。

![接続許可](./img/file_server_011.png)

〔7〕プロファイルの設定では現在の接続設定の項目にチェックを入れ、[次へ] をクリックします。　
※不明の場合はすべての項目にチェックを入れます。

![プロファイルの設定](./img/file_server_012.png)

〔8〕名前の設定では、名前に [icVaultServerFileTransfer] を入力し、説明に [icVaultファイル送受信サーバ] を入力します。

![名前の設定](./img/file_server_013.png)

[完了] をクリックし、終了します。。

<p class="note">〔8〕の名前は上記以外の任意の名前でも問題ありません。サーバ管理者が分かりやすい名前を付けても大丈夫です。</p>


### 送信の許可設定

〔1〕左側メニュー欄の [送信の規則] をクリックします。<br>
続いて、右メニュー [新しい規則] をクリックします。

![新しい規則](./img/file_server_014.png)

〔2〕[規則の種類] の設定では [プログラム] を選択し、[次へ] をクリックします。

![プログラム](./img/file_server_007.png)

〔3〕[このプログラムのパス(T):] にチェックし、[参照] をクリックします。

![プログラム設定](./img/file_server_008.png)

〔4〕icVaultServerFileTransfer のインストールパスに移動し、icVault FileTransfer Server.exe を選択し、[開く] をクリックします。<br>
※標準では C:\Program Files\CreativeMachine\icVaultServerFileTransfer にインストールされています

![操作の設定](./img/file_server_009.png)

〔5〕選択したパスが表示されたことを確認し、[次へ] をクリックします。

![プログラムの参照先設定](./img/file_server_010.png)

〔6〕[接続を許可する(A)] にチェックを入れ、[次へ] をクリックします。

![接続許可](./img/file_server_011.png)

〔7〕プロファイルの設定では現在の接続設定の項目にチェックを入れ、[次へ] をクリックします。　
※不明の場合はすべての項目にチェックを入れます。

![プロファイルの設定](./img/file_server_012.png)

〔8〕名前の設定では、名前に [icVaultServerFileTransfer] を入力し、説明に [icVaultファイル送受信サーバ] を入力します。

![名前の設定](./img/file_server_013.png)

[完了] をクリックし、終了します。。

<p class="note">〔8〕の名前は上記以外の任意の名前でも問題ありません。サーバ管理者が分かりやすい名前を付けても大丈夫です。</p>

以上で、外部との通信許可設定は完了です。
