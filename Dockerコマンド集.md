# Docker コマンドオプション集

## docker image捜索及び取得方法
`docker search 捜索キーワード`  docker hub上にあるimageの中から捜索、結果の(コンテナ名等)一覧を表示。<br>
>>例：docker search centOS<br>
>>どれがよくダウンロードされているか等表示されるので、便利

`docker pull コンテナ名` 　手元にdocker imageをダウンロード


### 一覧表示
`docker image`  存在する docker image　一覧を表示します。（docker pullなどで取得した手元にあるimageです）<br>
<br>
`docker ps` 　起動中のコンテナ一覧を表示します。 <br>
`docker ps -a` 　存在するコンテナ一覧を表示します。（起動中＋過去に起動し消去していないコンテナ） <br>

### 起動中のコンテナに入る
`docker attach コンテナID or コンテナ名`　// orはコマンドではないですよ！どっちを使ってもええということです！
>上記コマンドでコンテナ内に入った場合、（コンテナ内で）exitした時にコンテナは停止しコンテナから出ます。  
>>上記コマンドでコンテナ内に入ってしまったけれど、コンテナを”停止せず”にコンテナから出たい場合は <br>
>>`command+q` or `command+p`  <br>
>>でできます。<br>[注意]なぜか知りませんが、一回押しただけでは出れない時があります。

`docker exec -it コンテナID or コンテナ名 /bin/bash` <br>
>上記コマンドでコンテナ内に入った場合、（コンテナ内で）exitした時はコンテナは”停止せず”コンテナから出ます。<br>
>>attachよりこっちの方がええよ。マジで


