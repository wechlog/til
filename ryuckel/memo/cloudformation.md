# CloudFormation

AWS リソースの自動構築
構築されたリソース　＝　スタック

## スタック

テンプレートを分けることで、複数のスタックにリソースを分けることもできる

- IAM、CloudTrail 用スタック
- VPC、サブネット用スタック
  など

## CloudFormation テンプレート

JSON または YAML 形式で記載していく

画像

### セクション

- Resources セクション
  AWS リソースの設計を記載する
  リソースの型は Type で定義する
  型によって Propaties で設定する項目が決まる

- Parameters セクション
  実行時に入力する値を定義する
  Ref 関数で定義された値を参照することができる

- Mapping セクション
  Resouces セクション内で FindInMap 関数を用いて参照することで
  AMI ID を取得することができる

AWS::AccountId
AWS::Region

### 組み込み関数

- Ref 関数
  AWS リソースの定義された値を参照することができる
- FindInMap 関数
  Mapping セクションで定義した Map 型の変数を取得する
  Mapping の子要素、孫要素、値の項目と行ったように指定していく

例：[MappingName, Key1, Name1 ]

- Select 関数
  リストからインデックスを指定して値を取得する
- ImportValue 関数
  他の CloudFormation スタックの値を取得する
