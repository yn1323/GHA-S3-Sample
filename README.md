# GHA-S3-Sampleメモ

## やりた

- build後のコードをS3にアップロード
- アップロード後のURLをPRに追加コメント&既存のコメントの更新

## 前提条件

- S3には複数のbuild済みソースを設置する

## ポイント

- build後ソースが相対パスでasset等にアクセスできること
- S3のSecret Keyなどが必要
- 既存のコメント更新もよしなにやってくれる
- S3のオブジェクト期限が設定してあるとベター

## やったこと
  
[Workflow](.github/workflows/build.yml)に記載
