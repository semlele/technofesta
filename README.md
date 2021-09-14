# yy-lab テクノフェスタ　プロジェクト 
## これは, 2021年度静岡大学テクノフェスタにて展示予定のwebページです. 
## このリポジトリはGitHub Actions を用いて, コードを push する都度 S3 にアップロードされるようになってます. 

## 目次

- [ウェブサイトエンドポイント](#ウェブサイトエンドポイント)
- [バージョン管理について](#バージョン管理について)
- [注意点](#注意点)

## 詳細

### ウェブサイトエンドポイント

**[⬆ back to top](#目次)**

以下のページから, 吉井くんが作成したファイル (2021/9/14 時点 https://github.com/maasuke/techno-festa-yylab) を閲覧可能です.
(ドメイン名については, AWSの route53, CloudFront等を使って後に変えます. )

http://bucket-for-deploying-technofesta-project.s3-website-ap-northeast-1.amazonaws.com

### バージョン管理について

**[⬆ back to top](#目次)**

GitHub の設定とか諸々の観点から, 申し訳ないですが, バージョン管理はここのGitHubリポジトリ (https://github.com/semlele/technofesta) で行います.
今後は, ファイルの変更をして, それをwebブラウザ上で確認したい場合は, このリポジトリにコードを push して下さい.

### 注意点

**[⬆ back to top](#目次)**

ファイルの中身自体は変えてないですが, AWS側の都合でディレクトリ構造を変更しています. (src フォルダ内ファイルを編集するようにして下さい. )
そのためリポジトリに変更を加える場合は, まず自分のPCにリポジトリを丸ごとクローンしてからローカルで編集,  追加をした後, push することを勧めます.

## 参照
GitHub ActionsでウェブサイトをAmazon S3にデプロイする - DeveloperIO 

https://dev.classmethod.jp/articles/deploy-web-site-with-github-actions/

GitHub で他の人の Repository に参加する方法. 
GitHub 上の他の人の Repository のソースを修正して、修正の取り込み依頼(PULL リクエスト) を送るまでの流れ

https://www.engineer-memo.net/20200314-5576

このリポジトリをアップロードしている S3 バケット.

https://s3.console.aws.amazon.com/s3/buckets/bucket-for-deploying-technofesta-project?region=ap-northeast-1&tab=objects