# 名前
ひとこと掲示板「25ちゃん」

# 概要
名前、「ひとこと」を投稿できる掲示板です。
```bash
1 佐藤 2021-01-01 00:00:00
あけましておめでとうございます
2 汐 2021-01-01 00:00:01
おめでとう
```

# 動作環境
* Ubuntu20.04
* Python3
* MySQL8.0.23

# 事前準備
* $sudo apt install mysql-server
* $sudo pip3 install mysqlclient
* $sudo apt install apache2
* $sudo pip3 install python-dotenv

# 手順

* public_htmlディレクトリをユーザーディレクトリ下に作成
* リポジトリから 25chBBS.py を取得
* ~/public_html/に保存
* ~/public_html/に.envファイルを作成し以下を設定
```bash
bbs_db_host="ホスト名"
bbs_db_user="ユーザー名"
bbs_db_pass="パスワード"
bbs_db_name="データベース名"
```
* 取得したリポジトリのファイルに実行権限を付与
```bash
chmod 755 25chBBs.py
```
* ページを確認して反映されていたら完了

