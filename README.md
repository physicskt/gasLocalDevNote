# gasLocalDevNote
詳細なドキュメントや説明書は以下参照\
https://github.com/google/clasp

## Googleアカウントでclaspにログイン
次のコマンドを実行して、Googleアカウントでclaspにログインします。
```
clasp login
```

## PJのフォルダに移動

## よく使う clasp コマンドまとめ
| コマンド                                   | 説明                                               |
|--------------------------------------------|----------------------------------------------------|
| `clasp login`                              | Googleアカウントでログイン                         |
| `clasp logout`                             | ログアウト                                          |
| `clasp create --title "タイトル"`           | 新しいGASプロジェクトを作成                        |
| `clasp clone {スクリプトID}`                | 既存プロジェクトをクローン                          |
| `clasp push`                               | ローカルの変更をGASにアップロード                   |
| `clasp pull`                               | GAS側の最新コードを取得                             |
| `clasp open`                               | GASのWeb UIをブラウザで開く                         |
| `clasp deployments`                        | デプロイ済み一覧を確認                              |
| `clasp deploy --description "説明"`         | 新バージョンを作成してデプロイ                      |
| `clasp version`                            | バージョンだけ作成（デプロイなし）                  |
| `clasp undeploy {デプロイID}`               | デプロイを解除                                      |
| `clasp list`                               | 所有しているプロジェクト一覧を表示                   |
| `clasp status`                             | ローカルとGASの差分を確認                           |
| `clasp logs`                               | 実行ログを表示                                      |
| `clasp run {関数名}`                        | 指定した関数を実行                                  |

## GASプロジェクトのクローン
既存のプロジェクトを編集する場合は、プロジェクトのスクリプトIDを使用してクローンします。
スクリプトIDは、Apps Scriptエディタの「プロジェクト設定」から確認できます。
```
clasp clone {スクリプトID}
```

## 変更のプッシュ
スクリプトに加えた変更をGoogle Apps Scriptに反映させるには、以下のコマンドを使用します。
```
clasp push
```

## 初回デプロイ（バージョン作成 + デプロイ）
```
clasp deploy --description "初回デプロイ"
```

## 2回目以降の更新（再デプロイ）
```
clasp deploy --description "修正内容の説明"
```
```
clasp deploy --description "v1"  # デプロイしてバージョン作成
```

## 公開URLの確認（Webアプリの場合）
```
clasp deployments
```
