# GitHub Actions の初期設定
1. Settings -> Secrets and variables -> Actions -> Actions secrets and variables
1. New repository secret から下記を Environment secrets として追加する
- FTP_SERVER：FTPサーバ名（例：`https://example.com/`）
- FTP_USERNAME：FTPユーザ名
- FTP_PASSWORD：FTPパスワード
- FTP_SERVER_PRODUCTION_DIR：FTPサーバ内のテーマディレクトリを **/をつけて** 記述する（`/home/[FTPユーザ名]/www/[wpなど]/wp-content/themes/[テーマ名]/`）
- FTP_SERVER_DEVELOP_DIR：FTP_PRODUCTION_SERVERDIRと同様に記述する（例： `/home/[FTPユーザ名]/www/[developなど]/wp-content/themes/[テーマ名]/` ）

# Docker 環境の使用方法
1. Docker Desktop を起動する
1. `docker compose up`
1. http://localhost:8001 にアクセスする