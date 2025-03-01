# sample_app

Flutter のサンプルアプリです。

## Docker で開発環境構築

1. Android Studio をインストール
    - [Android Studio をインストールする](https://developer.android.com/studio/install?hl=ja)
2. Docker をインストール
    - [Docker Desktop for Mac](https://docs.docker.com/desktop/setup/install/mac-install/)
    - [Docker Desktop for Windows](https://docs.docker.com/desktop/setup/install/windows-install/)
3. リポジトリをクローン

    ```shell
    git clone https://github.com/hiromoo/flutter_sample_app
    ```

4. VSCode でリポジトリを開く
5. VSCode で以下の拡張機能をインストール
    - [Docker](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-docker)
    - [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
6. VSCode のコマンドパレット ( Command or Ctrl + Shift + P ) を開いて `Dev Containers: Reopen in Container` を選択
7. Android Studio > Device Manager からエミュレータを起動
8. Android エミュレータを接続

    ```shell
    adb connect host.docker.internal:5555
    ```

9. Android エミュレータ上に USB デバッグを有効化するかどうかを尋ねられるので、許可を選択

10. ビルド & 実行

    ```shell
    flutter run
    ```
