# スキルシート

## 基本情報

|key|value|
|----|----|
|名前|Takaharu Niki|
|現在地|大阪市|
|ブログ|[アントレプログラマー](https://entreprogrammer.jp/)
|X(Twitter)|[@takaharu_niki](https://twitter.com/takaharu_niki)|
|趣味|筋トレ・アニメ|

## 得意技術

### 言語

PHP || Python | Kotlin | Java | JavaScript || Go | TypeScript 

### フレームワーク

Laravel || Spring Boot | CakePHP | Next.js | React | Vue.js | jQuery

### RDB/NoSQL

MySQL || PostgreSQL | Redis | Memcached

### AWS

VPC | S3 | API Gateway | Lambda | ELB | EC2 | ECS | Fargate | Route53 | IAM | Cognito | RDS(MySQL) | Aurora | DynamoDB | ElastiCache(Redis|Memcached) | SNS | SES | CloudFormation | CloudWatch | EventBridge | Secrets Manager | Amplify | CodeBuild | CodeDeploy | CodePipeline 

### SaaS/PaaS
GitHub | GitHub Actions | BitBucket | Datadog

### その他
Docker | Jenkins | Fluentd | Ansible | Nginx | Apache | Gulp | Webpack | SASS

## 得意分野

SQLチューニング、TDDによる安全なコード変更、CI/CDによるチーム開発生産性の向上、IaCを用いた効率的なリソース管理、やらないことを見極める戦略的思考

## 主な業務経歴

### 宅食サービス事業会社(2021/09〜現在)

Laravelのアップグレード【Laravel】(2023/12〜2023/12)

【プロジェクト概要】Laravelアップグレードにおける計画と実行。

［担当業務］具体的には下記。
- 自動ツールLaravel Shiftの採用と実行
- Laravel Upgrade Guideに基づいた確認と修正。
- カナリアリリースを用いた影響を抑えたリリースの実施

postメソッドのAjax通信やモバイルアプリに不具合が発生した。
原因はセッションとキャッシュ用に同一ストレージを採用しているとアプリケーションはキャッシュを通してセッションデータを取得するが、キャッシュのキーに付与するプレフィックス変更を許容していたため。

AWS CodeDeployを使ったAuto Scaling対応【Fluentd/Datadog/S3/EC2/CodePipeline/CodeDeploy/CloudFormation】(2023/07〜11)

【プロジェクト概要】カナリアリリース等を目的に、DevOpsエンジニアとして技術選定と実施を担当。

［担当業務］EC2内の各種ログファイルデータのアーカイブ設定を担当。具体的には下記。
- 対象ログの選定
- ログごとのアーカイブ期間とアーカイブ先の決定
- EC2からS3への転送方法を調査・決定
- Fluentdのインストール、設定ファイルの作成、S３バケットへの転送確認
- Datadogの設定ファイル作成、Datadogへの転送確認

［担当業務］EC2内の設定ファイルをGitHubで管理。具体的には下記。
- 各インスタンスの差分を確認し、masterを最新化
- 各インスタンスへgit clone

［担当業務］CodeDeployの導入。具体的には下記。
- バッチサーバー用EC2インスタンスのデプロイ方法を、CodeDeployのインプレースデプロイへ変更
- CodePipeline・GitHub　Actionsを使用したデプロイ順序制御により、並列DBマイグレーションのエラーを回避
- Webサーバー用EC2インスタンスのデプロイ方法を、CodeDeployのAutoScalingグループを使用したブルーグリーンデプロイへ変更

入金消込システムの開発【Kotlin/Spring Boot/React/Laravel/AWS】(2023/04〜2023/06)

【プロジェクト概要】決算前業務の効率化のために、決済データと入金データを突合するシステムを開発

［担当業務］大量データ処理のパフォーマンスを考慮したシステム設計・実装・テストを担当。具体的には下記。
- 入金データを管理するテーブルを作成
- 入金データを外部APIから取得し、テーブルへ記録するバッチ処理を作成
- 突合用のテーブルを作成
- 突合用のテーブルへ、決済データと入金データを転記するバッチ処理を作成
- 突合用のテーブルからデータを取得するAPIを作成
- 突合結果を取得するUIを作成

決済代行会社変更のためのシステム開発【Laravel/AWS】(2023/01〜2023/03)

【プロジェクト概要】決済代行会社のサービス終了に伴う、システム改修。

［担当業務］決済システムの再設計・リファクタリングと新しい決済ロジックの導入を担当。具体的には下記。
- 度重なる決済会社変更と、それに伴うシステム改修で築かれた、ぼろぼろのシステムの現状を把握。
- 変更容易性を向上させるための設計と、既存システムへの影響調査。
- テスト駆動開発の実施による安全な変更
- 自動リファクタリングツールのRector導入と、スピード感のある変更の実施
- 新しい決済システムロジックの導入とリアーキテクチャ成功の証明

ECサイト・管理画面の機能開発【Laravel/JavaScript/AWS】(2021/09〜2022/12)

【プロジェクト概要】マーケティング施作実施や社内業務遂行を主な目的としたシステム開発。

［担当業務］フロント・バックエンドエンジニアとして設計・実装・テストを担当。

プロジェクト外の活動
- 採用活動
- 静的解析ツール、フォーマッターの導入
- 本番に追随するためのコンテナイメージのバージョンアップ
- ジョブの同期実行を目的としたメールコンテナの追加
- シークレットの管理のためにSecrets Managerを使用
- Secrets ManagerのシークレットをECSのタスク定義のsecretsに設定し、Spring Boot内で利用
- Findy Team+を使った、DevOps FourKeysの分析・改善

### レンタルサーバー事業会社(2019/09〜2021/08)

簡略化して記載

コンソール画面の追加・改修【Laravel/Vue.js/Zend Framework/Vanilla JS/CentOS/PostgreSQL】(1年5ヶ月)

［担当業務］実装とテストを担当

Windows ServerのOSテンプレートの開発　【OpenStack/CentOS/PostgreSQL】(4ヶ月)

［担当業務］テンプレートの作成と登録

VPSサービス用の追加テンプレートの新規開発【Ansible/CentOS/PostgreSQL】(3ヶ月)

［担当業務］Ansible Playbook作成、各種テストおよびplay book修正

