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

![スクリーンショット 2020-06-01 23 55 24](https://user-images.githubusercontent.com/36391432/83422102-ff4a5300-a463-11ea-8d42-ed5b104628c2.png)

![スクリーンショット 2020-06-01 23 55 30](https://user-images.githubusercontent.com/36391432/83422114-03767080-a464-11ea-91f1-10700e5ff6b3.png)

![スクリーンショット 2020-06-01 23 55 35](https://user-images.githubusercontent.com/36391432/83422120-05d8ca80-a464-11ea-977e-f8ecfd7250a0.png)

