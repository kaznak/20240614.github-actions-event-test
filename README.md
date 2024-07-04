# 20240614.github-actions-event-test

- プルリクを作ると environment を作成
- プルリクを閉じると対応する environment を削除

secret GH_TOKEN_ENVIRONMENT_OPERATION の設定が必要。パーミッションは以下の通り:

- Read access to metadata(mandate)
- Read and Write access to actions variables(variables)
- Read and Write access to administration
- Read and Write access to environments

## メモ

### 命名規則

名前はスネークケース。
キーワードはケバブケース。

### push

- 手動で push するとトリガー
- プルリクがマージされてもトリガーされる

### pull_request

- pull request 関連のアクションでトリガー
- 起動時にコンフリクトがあるとトリガーされない

### pull_request

- pull request 関連のアクションでトリガー
- 起動時にコンフリクトがあってもトリガーされる
