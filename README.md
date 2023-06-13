環境構築手順

1.node.jsをPCへインストール
    公式サイト参照：https://nodejs.org/ja/
2.dockerのインストール
    公式サイト参照：https://matsuand.github.io/docs.docker.jp.onthefly/get-docker/
3.環境構築
    任意の開発用ディレクトリ作成
    vscodeインストール：https://azure.microsoft.com/ja-jp/products/visual-studio-code
    vscodeで開発用ディレクトリを開く（任意のファイルを新規作成して学習用とすると便利かもしれません）
    gitより開発環境をクローン
        →左のアイコン上から三番目クリック
        →「リポジトリのクローン」をクリックして「https://github.com/UT-T/training.git」と入力
    左のアイコンの一番上をクリックし、ファイルが複製されたことを確認する
    dockerのインストール：https://matsuand.github.io/docs.docker.jp.onthefly/get-docker/
    vscodeのターミナルを見えるようにする
        →下の青いラインの上辺をドラッグで持ち上げる
        →エクスプローラーより右側
    ターミナルにてクローンしてきたファイル（デフォルトの場合「react」）をカレントディレクトリにする
        →cd react
    下記コマンドを入力しEnterでコンテナ作成
        →docker-compose up -d --build
    任意のブラウザで下記のURLを設定してサンプロ画面を表示
        http://localhost:3000    
        
        サンプルページが表示されなかった場合は下記のコマンドを叩いて再表示してみてください
            docker compose logs -f
        出力されるログの中に「Local:http://localhost:3000」の文言が表示されたら下記URLを確認するとデモページが表示される

次回以降の開発環境の起動方法
    dockerアプリを起動する
    vscodeで開発用ディレクトリを開く
    ターミナルにてクローンしてきたファイル（デフォルトの場合「react」）をカレントディレクトリにする
        →cd react
    下記コマンドを入力しEnterで初回に作成したコンテナを起動
        →docker-compose up -d
    サンプルアプリを起動する（初回の場合は不要でした）
        docker compose logs -f
    出力されるログの中に「Local:http://localhost:3000」の文言が表示されたら下記URLを確認するとデモページが表示される