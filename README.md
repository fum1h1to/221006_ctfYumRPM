# ctfYumRPM
dockerで自作RPMパッケージを自前のYumリポジトリで公開する環境を作った。<br>また、CTFのような形式にもなっているので、```flag{..}```形式のフラッグを見つけてみてください。

# Usage

1. Dockerをインストールする

2. コンテナの作成
    ```
    $ docker-compose up -d
    ```

3. クライアントの起動

    ```
    $ docker exec -it ctfYumRPM_client
    ```

4. クライアントに自作パッケージである```ctfYumRPM```をインストール

    ```
    $ yum install -y ctfYumRPM
    ```

5. ```flag{..}```という形式でどこかにフラッグがあるので、探す。