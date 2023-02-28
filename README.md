環境構築手順

1.node.jsをPCへインストール
    公式サイト参照：https://nodejs.org/ja/
2.dockerのインストール
    公式サイト参照：https://matsuand.github.io/docs.docker.jp.onthefly/get-docker/
2.環境構築
    任意の開発用ディレクトリ作成
    vscodeインストール：https://azure.microsoft.com/ja-jp/products/visual-studio-code
    vscodeで開発用ディレクトリを開く
    gitより開発環境をクローン
        →左のアイコン上から三番目クリック
        →「リポジトリのクローン」をクリックして「https://github.com/UT-T/training.git」と入力
    左のアイコンの一番上をクリックし、ファイルが複製されたことを確認する
    dockerのインストール：https://matsuand.github.io/docs.docker.jp.onthefly/get-docker/
    vscodeのターミナルを見えるようにする
        →下の青いラインの上辺をドラッグで持ち上げる
        →エクスプローラーより右側
    ターミナルにて下記コマンドを入力しEnterでコンテナ作成
        →docker-compose up -d --build
    サンプルアプリを起動する
        docker compose logs -f
    出力されるログの中に「Local:http://localhost:3000」の文言が表示されたら下記URLを確認するとデモページが表示される
        http://localhost:3000