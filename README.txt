# Hero Video Patch (for GitHub Pages static site)
この2ファイルをリポジトリにアップし、動画ファイルを `video/IMG_4835.mov` に置くと、
トップのヒーローが動画になります（自動再生/ミュート/ループ/モバイル対応）。

## 手順
1. GitHub で `video/` フォルダを作成（例: `Add file` → `Create new file` で `video/.gitkeep` を作り Commit）
2. `video/` に `IMG_4835.mov` をアップロード
3. リポジトリのルートにある `index.html` と `styles.css` を、このパッチのファイルで置き換えて Commit
4. 公開ページを Shift＋再読み込み

### 動画再生のコツ
- 自動再生は **muted + playsinline** が必須（iOS含む）
- 互換性UPのため、可能なら **MP4(H.264/AAC)** 版も用意して `<source>` を追加してください
- GitHubは 100MB を超えるファイルの push を拒否します。大きい場合は圧縮（1080p→720p, 8Mbps→4〜6Mbps 等）を検討してください
