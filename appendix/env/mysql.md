# MySQLのインストール

### Installing MySQL Server on Windows

ここでは、MySQL Community Serverのインストール方法を説明します。

1. MySQL Community Serverのインストーラをダウンロードするためには、公式サイトのダウンロードページ（[https://dev.mysql.com/downloads/mysql/](https://dev.mysql.com/downloads/mysql/)）にアクセスします。
2. 「Download」ボタンは複数ありますが、「Windows (x86, 64-bit), MSI Installer」をダウンロードします。&#x20;
3. 「No thanks, just start my download.」を選択するとダウンロードが始まります。
4. ダウンロードした「mysql-9.1.0-winx64.msi」を実行すると、インストーラが起動します。もし「This application requires Visual Studio 2019 x64 Redistributable. Please install the Redistributable then run this installer again.」と表示された場合は、下記のNoteを参照してください。
5. セットアップの画面が表示されたら、Next\*クリックします。&#x20;
6. ライセンスが表示されたら、「I accept the terms in the License Agreement」にチェックを入れ、「Next」をクリックします。&#x20;
7. セットアップの種類を選択します。ここでは、「Typical」を選択し、「Next」をクリックします。&#x20;
8. 「Install」をクリックします。&#x20;
9. 「Run MySQL Configurator」にチェックを入れている状態で、「Finish」をクリックします。&#x20;

:::{note} MySQL Community Serverをインストールするには、Microsoft Visual C++再頒布可能パッケージが必要です。 公式サイト（[https://learn.microsoft.com/ja-jp/cpp/windows/latest-supported-vc-redist?view=msvc-170](https://learn.microsoft.com/ja-jp/cpp/windows/latest-supported-vc-redist?view=msvc-170)）にアクセスし、「最新のMicrosoft Visual C++再頒布可能パッケージ」をダウンロードしてインストールしてください。「X64」、「x86」と「ARM64」の3つがありますが、CPUのアーキテクチャに合わせて適切なものを選択してください。 :::

以上でMySQL Community Serverのインストールが完了しましたが、続いてMySQL Configuratorの設定を行います。

### MySQL Configuratorの設定

1. MySQL Community Serverのインストールが完了したら、MySQL Configuratorが自動的に起動します。「Next」をクリックします。&#x20;
2. 「Next」をクリックします。&#x20;
3. ここでは「Type and Networking」を設定します。デフォルトのまま次へ進みます。&#x20;
4. 「Accounts and Roles」の画面では、Rootアカウントのパスワードの設定を行います。「MySQL Root Password」と「Rpeat Password」に同じパスワードを入力し、「Next」をクリックします。&#x20;
5. デフォルトのまま「Next」をクリックします。&#x20;
6. 「Next」をクリックします。&#x20;
7. 必要に応じて、Sample databasesを選択し、「Next」をクリックします。&#x20;
8. 「Execute」をクリックします。&#x20;
9. 実行が完了したら、「Next」をクリックします。&#x20;
10. 「Finish」をクリックします。&#x20;

以上でMySQL Community Serverのインストールが完了しました。

### MySQL Command Line Clientの起動

インストールが完了したら、スタートメニューから「MySQL 9.1 Command Line Client」を起動します。&#x20;

クライアントが起動すると、パスワードの入力を求められますので、先ほど設定したMySQL Root Passwordを入力します。以下のように表示されたら、MySQL Serverに接続できています。&#x20;
