# Code シリーズ

## 利用シーン

1. ソースを CodeCommit のリポジトリへプッシュ
2. CodeBuild でビルド
3. テスト(CodeDeploy)
4. OK
5. CodeDeploy でデプロイ
   ※CodePipeline でプロセスを統合

## CodeCommit

Git の標準機能を持っていて、プルリクエストの対応も可能

### リポジトリ

ソースコードの保存場所
既存の Git リポジトリからの意向も可能

ファイル編集には CodeCommit コンソール、AWS CLI、CodeCommitAPI を使用する

CodeCommit のユーザー認証設定

- IAM ユーザーとの関連付けで行う
  - 発行されたユーザー名とパスワードで Git の認証を行う
  - IAM ポリシーで特定のブランチへのプッシュやマージの制限も可能
- 通信暗号化
  - HTTPS,SSH を使用
  - リポジトリのソースコードは KMS キーによって暗号化される

### 他のサービスと連携

- CloudTrail と連携して AWS で発行される CodeCommitAPI の利用状況を S3 に保存する
- SNS に通知
- トリガー(リポジトリへのプッシュなど)を設定し Lambda 関数を実行する

## CodeBuild
