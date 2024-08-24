# actions_aws_deploy

GitHub Actions で main ブランチに push したら、Pages と AWS S3 へデプロイする

デプロイ先
https://d25oh4ofh00dp6.cloudfront.net/

https://den2k6.github.io/actions_aws_deploy/

## プロジェクトの概要

このプロジェクトは、GitHub ActionsとAWS S3を使用して、自動デプロイメントプロセスを実装しています。mainブランチにプッシュされると、コンテンツが自動的にGitHub PagesとAWS S3にデプロイされます。

## デプロイ先

1. AWS CloudFront: https://d25oh4ofh00dp6.cloudfront.net/
2. GitHub Pages: https://den2k6.github.io/actions_aws_deploy/

## 機能

- GitHub Actionsによる自動デプロイ
- AWS S3を使用したホスティング
- CloudFrontによるコンテンツ配信

## 使用技術

- GitHub Actions
- AWS S3
- AWS CloudFront
- HTML/CSS

## セットアップ手順

1. このリポジトリをクローンする
2. 必要な環境変数をGitHubシークレットに設定する
3. mainブランチにプッシュしてデプロイをトリガーする

## 貢献方法

プルリクエストは歓迎します。大きな変更を加える場合は、まず問題を開いて議論してください。
