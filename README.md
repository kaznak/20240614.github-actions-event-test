# 20240614.github-actions-event-test

- プルリクを作ると environment を作成
- プルリクを閉じると対応する environment を削除

## トリガのメモ

### push

- 手動で push するとトリガー
- プルリクがマージされてもトリガーされる

### pull_request

- pull request 関連のアクションでトリガー
- 起動時にコンフリクトがあるとトリガーされない

### pull_request

- pull request 関連のアクションでトリガー
- 起動時にコンフリクトがあってもトリガーされる
