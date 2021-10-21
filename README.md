# yy-lab テクノフェスタ　プロジェクト (README 2021/10/15 更新)
## これは, 2021年度静岡大学テクノフェスタにて展示予定のwebページです. 
## このリポジトリはGitHub Actions を用いて, コードを push する都度 S3 にアップロードされるようになってます. 

## 目次

- [ウェブサイトエンドポイント](#ウェブサイトエンドポイント)
- [バージョン管理について](#バージョン管理について)
- [注意点](#注意点)

## 詳細

### ウェブサイトエンドポイント

**[⬆ 目次](#目次)**

以下のページから, 吉井くんが作成したテンプレートベースで作成したファイル (2021/10/15時点) を閲覧可能です.

ドメイン名については, AWSの route53を用いて独自ドメイン取得, 設定を行なっています. 

AWS Certificate Manager を使ってSSL証明書を発行し, httpsで公開しています. 


https://yy-techno-festa.net

### バージョン管理について

**[⬆ 目次](#目次)**

GitHub の設定とか諸々の観点から, 申し訳ないですが, バージョン管理はここのGitHubリポジトリ (https://github.com/semlele/technofesta) で行います.
今後は, ファイルの変更をして, それをwebブラウザ上で確認したい場合は, このリポジトリに pull request して下さい.

※ warning ※ 

pull requestが正しく行われていないようです. 

現状, folk先のリポジトリのsrcファイルを都度DLして反映させている状態です.

下記のサイトを参照しながら行えば, 問題なく出来ます. 

### 注意点

**[⬆ 目次](#目次)**

ファイルの中身自体は変えてないですが, AWS側の都合でディレクトリ構造を変更しています. (src フォルダ内ファイルを編集するようにして下さい.)

Landing Page の名前は "index.html" のままで変更しないで下さい. 


## 参照
GitHub ActionsでウェブサイトをAmazon S3にデプロイする - DevelopersIO 

https://dev.classmethod.jp/articles/deploy-web-site-with-github-actions/

【AWS】S3+CloudFront+Route53+ACMでSSL化(https)した静的Webサイトを公開する - Zenn

https://zenn.dev/wakkunn/articles/66a6e8372611dc

GitHub で他の人の Repository に参加する方法. 
GitHub 上の他の人の Repository のソースを修正して, 修正の取り込み依頼(PULL リクエスト) を送るまでの流れ.

https://www.engineer-memo.net/20200314-5576

このリポジトリをアップロードしている S3 バケット

https://s3.console.aws.amazon.com/s3/buckets/yy-techno-festa.net?region=ap-northeast-1&tab=objects