# RStudio-Docker
DockerでR Studio環境を構築するやつ
## 使い方
立ち上げて  
`docker-compose up -d`

ブラウザ上で使う  
`http://localhost:8703`

資格情報は以下の通り
- ID : rstudio
- PW : password

やめる  
`docker-compose stop`

データを消す  
- `src/`以下を空にする
- `docker-compose down -v`

srcフォルダはコンテナ内のホームディレクトリにマウントされます。
利用するファイルを出し入れできます。

## 利用イメージ
[rocker/tidyverse](https://hub.docker.com/r/rocker/tidyverse)
