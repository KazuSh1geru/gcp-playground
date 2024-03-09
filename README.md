# gcp-playground
Google Cloud のリソースで遊ぼう。

## Cloud Functions

### デプロイ（gcloud コマンド）

hello_get 関数をデプロイする。
```bash
gcloud functions deploy python-http-function \
--gen2 \
--project=your-project-id \
--runtime=python311 \
--region=asia-northeast1 \
--source=. \
--entry-point=hello_get \
--trigger-http
```