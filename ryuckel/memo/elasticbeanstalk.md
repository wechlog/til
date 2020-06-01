# ElasticBeansTalk

定番のインフラ構成を自動構築する

## 定番構成

- Web サーバー構成(ELB+AutoScalingGroup+EC2)
- Bacth ワーカー構成(SQS+AutoScalingGroup+EC2)

それぞれ、低コストの構成か、高可用性の構成から選択ができる
高可用性の場合は、最大のサーバーの台数を決められたりする

## 利用方法

マネジメントコンソール以外にも、Eclipse から事項する AWS Toolkit for Eclipse が提供されている
また、EB CLI(Elastic BeansTalk 専用の CLI)もある

## デプロイのサポート

画像
