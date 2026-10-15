# Active School Travel | 科研費研究成果ページ

このリポジトリは、東京大学の研究室ホームページ内に設けた科研費特設コーナーの**子ページ**を管理するものです。

- 親ページ（研究概要・目次）：https://ua.t.u-tokyo.ac.jp/active-school-travel/
- GitHub Pages（子ページ）：https://hino-kimihiro.github.io/active-school-travel/
- 1-3 日本版移動自由性尺度の提案：`1-3/index.html`

## 構成
- `index.html`：WordPress親ページへの転送専用
- `css/style.css`：各子ページ共通のCSS
- `1-3/index.html`：完成見本
- `template/index.html`：新規ページの制作開始用テンプレート
- `各番号/index.html`：番号ごとの研究成果ページ（例：`1-4/index.html`）

## 学生の制作・校正手順
1. 執筆者から提供されたPPTXを参照し、`1-3/index.html`と`template/index.html`の形式に合わせて新規ページを作る。
2. 作業用ブランチでページ別のフォルダを追加する。本文は`index.html`、図は各ページの`images/`に保存する。
3. 共通デザインは`css/style.css`を使用し、ページごとにスタイルを無断で変更しない。
4. プレビューで本文・図表・注記・スマートフォン表示・「親ページに戻る」リンクを確認する。
5. 執筆者に確認を依頼し、回答・修正状況を記録する。
6. Pull Requestを作り、代表者の確認後に`main`へ統合する。

**注意**：公開リポジトリなので、未公開の原稿、個人情報、メール、機密資料を置かないこと。公開用の著作物についても権利を確認すること。

## 運用上の注意
当初移植した1-3の図は、表示のため大学WordPress上の画像を参照しています。今後は可能ならGitHubにも画像を保存し、相対パスに変更してください。移行完了まではWordPress側の画像を削除しないでください。
