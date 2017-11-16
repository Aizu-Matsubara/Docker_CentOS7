# CentOS7へのDocker導入メモ

## インストール
インストールコマンド 
'$ sudo yum install -y docker'

※これは CentOS7の公式リポジトリで「docker」という名前のパッケージが配布されているため　2017/09現在
※確か実行バイナリファイルのやつはそのままではCentOS7では使えなかった？
※sudoはroot権限が必要。管理者（root)になるか、
$ su
管理者のパスワード入力
$ yum install -y docker
$ exit
でインストール。どのみちあとあと面倒なので、管理者権限は持っておくこと。
