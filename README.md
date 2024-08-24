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

1. このリポジトリをクローンする
2. 必要な環境変数をGitHubシークレットに設定する
   - AWS_ACCESS_KEY_ID
   - AWS_SECRET_ACCESS_KEY
   - AWS_REGION
   - S3_BUCKET_NAME
3. mainブランチにプッシュしてデプロイをトリガーする

## ファイル構造

- `docs/index.html`: メインのHTMLファイル
- `docs/styles.css`: スタイルシート
- `.github/workflows/deploy.yml`: GitHub Actionsワークフローファイル

## 貢献方法

プルリクエストは歓迎します。大きな変更を加える場合は、まず問題を開いて議論してください。

## 備考

アクセスキー更新