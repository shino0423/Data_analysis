# Dockerを利用したJupyterLAｂ開発環境の構築
```
---------windows---------               ----Docker Container----
| ./py3/root_jupyter    |               |  /root/.jupyter       |               
| ./workspace           |               |  /workspace           |               
|  ---------------      |               |  ---------------      |
| │ Browser       │     |==(port:8080)==| │ Jupyter Lab   │     |
| │               │     |               | │ Python        │     |
| ----------------      |               | ----------------      | 
-------------------------               -------------------------
```
## フォルダ構成
```
├ py3           　      # Pythonサービス用フォルダ
│ ├ root_jupyter　      # JupyterLabの設定を永続化するためのフォルダ
| └ Dockerfile          # Pythoサービス用のDockerfile
├ workspace             # JupyterLabの作業フォルダ
├ docker-compose.yml    # 船体を管理するdocker-compseの設定
└ up-sown.cmd           #　コンテナの起動停止を簡単に行うためのバッチ
```

## 開発環境の展開
コマンドプロンプト等で以下のコマンドを実行する
```
start ./up-down.cmd
```