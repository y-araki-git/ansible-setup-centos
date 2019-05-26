# CentOS用 Ansible セットアップサンプル

AnsibleでCentOSの自動セットアップ。  
環境に応じてインストールするパッケージやバージョンは変更。  
サンプルは管理ユーザをadmuser、開発用ユーザをdevuserとしている。  
メインの実行ファイルを作成して、各ymlファイルをインクルードする形で進めるとよい。  

  - 構成
  
  ├Apache22.yml              # Apacheインストール  
  ├default.yml               # OS初期設定(共通設定)  
  ├java.yml                  # Javaインストール  
  ├mysqlclient.yml           # MySQL Client5.7インストール  
  ├nginx.yml                 # nginxインストール・設定  
  ├node-exporter.yml         # node-exporterインストール・設定 ※監視サーバとしてPrometheusを使用している場合。  
  ├php72.yml                 # php7.2関連インストール  
  ├pyenv-install-python.yml  # pyenvインストール  
  ├pyenv.yml                 # devuser用python実行環境設定  
  └python35ius.yml           # python35u,関連モジュールインストール  
