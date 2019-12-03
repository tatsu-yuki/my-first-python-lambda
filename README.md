## はじめてのPython-Lambda勉強用リポジトリ

## ディレクトリ構成
- `users`
    - `get.py` ... ユーザ一覧取得(`GET /users`)
    - `post.py` ... ユーザ作成(`POST /users`)
    
- `users-userid`
    - `get.py` ... ユーザ取得(`GET /users/{user_id}`)
    - `put.py` ... ユーザ更新(`PUT /users/{user_id}`)
    - `delete.py` ... ユーザ削除(`DELETE /users/{user_id}`)

    
## 事前準備
- [Python3.7.x](https://www.python.org/downloads/release/python-375/)のインストール
- [AWS CLI](https://docs.aws.amazon.com/ja_jp/cli/latest/userguide/install-windows.html)インストール
- AWS CLI認証情報設定
```
$ aws configure
AWS Access Key ID [****************YFXQ]: {AWS IAMで払い出したアクセスキー}
AWS Secret Access Key [****************5cqJ]: {AWS IAMで払い出したシークレットアクセスキー}
Default region name [ap-northeast-1]: ap-northeast-1
Default output format [json]: json
```

- [npmインストール](https://nodejs.org/en/)
- Serverless Frameworkインストール
```
$ npm install -g serverless
```


## デプロイ
deployしたい `serverless.yml` と同ディレクトリで以下のコマンドを実行。
```
$ sls deploy -v
```
