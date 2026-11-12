# ar-models

スマホのカメラで AR として見られる 3D モデル置き場。
[model-viewer](https://modelviewer.dev/) + GitHub Pages で配信しています。

**公開URL:** https://masa-nova.github.io/ar-models/

## 中身

| ファイル | 容量 | ポリゴン | 用途 |
|---|---|---|---|
| `gumball-robot-ar.glb` | 2.84 MB | 79,410 | 本番（ページが読む） |
| `gumball-robot-light.glb` | 1.34 MB | 39,706 | 回線が細い時の予備 |

元データは 46.9 MB / 1,985,394 ポリゴン。Google の Scene Viewer 推奨値
（10万ポリ以下・10MB以下・JPEG・2048px以下）に収まるよう圧縮しています。

## モデルを追加するとき

1. サブフォルダを作る（例 `airship/`）
2. `index.html` をコピーして `src` を差し替える
3. push すると `https://masa-nova.github.io/ar-models/airship/` で公開される

## 動作条件

- **HTTPS 必須**（AR はローカルファイルや http では起動しません）
- Android: Chrome ＋ ARCore 対応端末
- iPhone: Safari（iOS 12 以降）
- パソコンでは AR ボタンは出ません
