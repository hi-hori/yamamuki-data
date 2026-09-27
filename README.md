# Yamamuki data

やまむきのオフラインデータ専用リポジトリです。アプリのソースコードと再生成ツールは
https://github.com/hi-hori/yamamuki の codex/terrain-display ブランチにあります。

- terrain.zip: 陰影地形・海・湖・河川の内蔵パック（Git LFS）
- peaks.zip: 山頂の内蔵パック
- history/: ソースコードの過去コミットが参照する地形パック（Git LFS）
- *.sha256: 最新パックのSHA-256
- NOTICE.txt / PEAKS-NOTICE.txt / ODbL-1.0.txt: 出典とライセンス。各パック内にも収録しています。

アプリ側の .lfsconfig はこのリポジトリをLFS保存先として参照します。
新規clone時はGit LFSをインストールしてください。既存cloneでは git lfs pull で取得できます。
データ更新時はアプリ側で再生成・検証し、LFSをpushしてください。
このリポジトリの最新パック参照・ハッシュも同じ版へ更新してください。
