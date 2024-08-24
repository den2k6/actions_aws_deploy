# actions_aws_deploy

GitHub Actions で main ブランチへの push をトリガーに AWS S3 と GitHub Pages へデプロイします。

## デプロイ先

1. AWS CloudFront: https://d25oh4ofh00dp6.cloudfront.net/
2. GitHub Pages: https://den2k6.github.io/actions_aws_deploy/

## プロジェクトの概要

このプロジェクトは、GitHub ActionsとAWS S3を使用して、自動デプロイメントプロセスを実装しています。mainブランチにプッシュされると、コンテンツが自動的にGitHub PagesとAWS S3にデプロイされます。

## 機能

- GitHub Actionsによる自動デプロイ
- AWS S3を使用したホスティング
- CloudFrontによるコンテンツ配信
- シンプルなHTML/CSSデザイン

## 使用技術

- GitHub Actions
- AWS S3
- AWS CloudFront
- HTML/CSS

## セットアップ手順

1. AWSコンソールでIAMユーザーを作成し、アクセスキーを生成する
2. AWS S3でバケットを作成する
3. AWS CloudFrontでディストリビューションを作成する
   - オリジンアクセスコントロール（OAC）を設定し、S3バケットにバケットポリシーを適用する
4. GitHubで新しいリポジトリを作成する
5. ローカル環境にリポジトリをクローンする
6. 以下の環境変数をGitHubシークレットとして設定する
   - AWS_ACCESS_KEY_ID
   - AWS_SECRET_ACCESS_KEY
   - AWS_REGION
   - S3_BUCKET_NAME
   - CLOUDFRONT_DISTRIBUTION_ID
7. リポジトリの設定でGitHub Pagesを有効にする
8. `.github/workflows`フォルダを作成し、デプロイ用のワークフローファイル（例：`deploy.yml`）を設定する
9. `docs`フォルダを作成し、Webサイトのコンテンツ（HTML、CSS、JavaScript等）を配置する
10. 変更をコミットし、mainブランチにプッシュしてデプロイをトリガーする

## ファイル構造

- `docs/index.html`: メインのHTMLファイル
- `docs/styles.css`: スタイルシート
- `.github/workflows/deploy.yml`: GitHub Actionsワークフローファイル

## 貢献方法

プルリクエストは歓迎します。大きな変更を加える場合は、まず問題を開いて議論してください。

## 備考

1. アクセスキー更新2
1. workflows に CloudFront のキャッシュ削除を追加
1. バージョン追記

* Ver. 0.10