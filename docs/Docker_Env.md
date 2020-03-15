# Docker 環境構築手順

## Dockerのインストール(Mac編)

1. 下記URLへアクセスし、「Docker For Mac」のダウンロードを行う.
 https://store.docker.com/editions/community/docker-ce-desktop-mac

2. 画面右下にある「Get Docker」ボタンをクリックしてインストール開始

3. 2.でダウンロードしたdmgファイルを開き、Docker For MacのアイコンをApplicationフォルダにドラッグ&ドロップ

4. Applicationフォルダ内にあるDocker For Macをさらにダブルクリック. 初回起動時のため警告ダイアログが表示されるが気にせず、「OK」ボタンをクリック.

5. Welcomeメッセージが表示されたら、「Next」ボタンをクリック.

6. privileged(管理者権限)アクセスが必要な旨のダイアログが表示されるので、「OK」ボタンをクリック

7. privileged(管理者権限)アクセスを承認するために管理者権限を持つアカウントのパスワードを入力し、「ヘルパーを追加」をクリック.

8. 7.まで完了するとDocker For Macが起動し、ポップアップが表示され「Docker is starting...」のメッセージが表示される.

9. 時間が経つと「Docker is now up and runnnig!」と表示される.

10. 9.まででインストールとDockerの起動が完了したことを確認するためターミナルを開き、下記コマンドを実行し、ClientとServerが表示されたら正常に完了しています.

-- Docker バージョン確認
 docker version
-- Docker Compose バージョン確認
 docker-compose version


## Dockerのインストール(Windows編)

1. 下記URLへアクセスする.
 http://www.docker.com/products/docker-toolbox

2. 「Download for Windows」ボタンをクリックし、インストールを行う.

3. 2.でダウンロードしたDocker Toolboxを実行

4. デバイス許可を求めるダイアログが表示されるので「はい」をクリック.

5. インストールウィザードを開いたら、「Next」をクリック.

6. インストール先を確認されるが、問題なければデフォルトのまま「Next」をクリック.

7. インストールするコンポーネントを選択する.デフォルトのまま「Next」をクリック.

8. 追加タスクの確認をする.デフォルトのまま「Next」をクリック.

9. インストール確認画面が表示される.問題なければ「Install」をクリック.

10. インストールが始まるので、完了するまで待ちます.

11. インストール途中で、デバイスソフトウェアのインストール確認が入るが「インストール」を選択し、進める.

12. インストールが完了したら「Finish」をクリック.

13. Docker Quickstart Terminalを開く.

14. Docker Quickstart Terminalの初回実行時、docker-machineコマンドにより、defaultという名前のDocker実行用の仮想マシンがVirtualBox上に作成される.

15. 途中VirtualBoxのデバイス変更許可のダイアログが表示されるが「はい」を選択.

16. docker-machineの実行が完了したらDocker実行のターミナル画面が表示される.

17. 下記コマンド入力し、実行する.インストールが正常完了していることを確認する.

 docker version

18. 下記コマンドよりhello-worldのDockerイメージを実行し、コンテナの動作確認を行い、正常に動作したらDocker及びDocker ToolBoxのインストールは完了.

 1. docker run hello-world
 2. docker run -it ubuntu bash
