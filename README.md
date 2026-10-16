# Active School Travel | 科研費研究成果ページ

このリポジトリでは、研究室ホームページ内の科研費特設コーナーの**子ページ**を制作・管理します。執筆者の提出したPPTXを基に、AIを活用してHTMLを作成し、執筆者の確認と修正への対応までを行います。

## 作業に使うURL

- [WordPress親ページ（研究概要・目次）](https://ua.t.u-tokyo.ac.jp/active-school-travel/)
- [GitHubリポジトリ（ファイル管理）](https://github.com/hino-kimihiro/active-school-travel)
- [GitHub Issues（担当・進捗管理）](https://github.com/hino-kimihiro/active-school-travel/issues)
- [GitHub Pull Requests（変更のレビュー）](https://github.com/hino-kimihiro/active-school-travel/pulls)
- [完成見本 1-3：日本版移動自由性尺度の提案](https://hino-kimihiro.github.io/active-school-travel/1-3/)

## 1. 最初にすること

1. GitHubの共同編集招待を承諾する。
2. 上記の完成見本と、`1-3/index.html`、`template/index.html`、`css/style.css` を確認する。
3. [Issues](https://github.com/hino-kimihiro/active-school-travel/issues)から担当ページを確認する。現在の目次は暫定的に22件で、後から増減する。
4. 担当ページのPPTXと公開可能な図表を、大学の共有ストレージで確認する。PPTXそのものをGitHubに置かない。

## 2. PPTXからHTMLへの変換

- 各ページに `番号/index.html`（例 `2-1/index.html`）を用意し、図表は `番号/images/` に保存する。
- `template/index.html` を複製し、完成見本1-3の文字サイズ、見出し、Key points、図表の体裁に合わせる。
- AIを使用してよいが、研究結果・数値・出典・解釈を創作したり変更したりしない。疑問点は執筆者への確認事項として残す。
- 共通デザインは `css/style.css` を利用し、独断で変更しない。
- 画像は原則リポジトリ内に保存し、`images/figure1.png` などの相対パスで参照する。
- 外部資料の転載、個人情報、非公開データなどが含まれないことを公開前に確認する。

**AIへの指示例**：「添付のPPTXをもとに、完成見本1-3と共通HTMLテンプレートに沿って研究成果紹介ページを作成してください。数値や研究内容を変えず、元資料にない主張や出典を加えないでください。図表の見出し・キャプションを保ち、不明点は別途列挙してください。」

## 3. 作業ブランチと公開

1. 担当ページごとに作業ブランチ（例 `page/2-1`）を作り、ファイルを編集する。`main` を直接変更しない。
2. PC・スマートフォンで本文、図表、リンク、誤字、表示を確認する。
3. Pull Requestを作成し、他の共同編集者のレビューを受けて`main`に統合する。現在のRulesetでは1件の承認レビューが必要。
4. 統合後、GitHub PagesのURL（例 `https://hino-kimihiro.github.io/active-school-travel/2-1/`）を確認する。

**専用プレビュー環境は設けません。** 初稿もGitHub Pagesで閲覧できる状態にしますが、執筆者と研究代表者の確認が終わるまでは、WordPress親ページの目次からリンクしません。リンクがなくてもページ自体は一般公開されるため、未公開原稿、秘密情報、許諾のない図表はGitHubに登録しないこと。

## 4. 執筆者確認と修正

1. 研究代表者と相談して、GitHub PagesのURLを執筆者に送り、内容・数値・図表・表現・公開可否を確認する。
2. 修正不要の場合も含め、回答日を担当Issueに記録する。
3. 修正があれば新たな作業ブランチとPull Requestで反映し、必要に応じて再確認する。
4. 未回答の執筆者への催促は、研究代表者と相談して行う。
5. 最終的に研究代表者が確認し、親ページからリンクを追加する。**このリンク追加を正式公開の区切りとします。**

## 5. Issuesの管理方法

- 各ページのIssueに担当学生・ステータス・確認依頼日・回答日・修正内容を記録する。
- チェックリストには「HTML初稿」「画像保存」「表示確認」「執筆者確認」「修正完了」「代表者確認」「親ページリンク追加」までの状況を残す。
- Issueのタイトルやページ数は変更可能。担当が未定のIssueは学生を招待してから割り当てる。
- メール本文、非公開原稿、個人情報はIssueに転載しない（Issueも公開される）。

## 6. 重要な注意

- `index.html`（リポジトリ直下）はWordPress親ページへの転送専用であり、原則変更しない。
- 1-3の画像2点はすでに `1-3/images/` に保存されており、WordPressの画像への依存は解消済み。
- 研究内容の最終判断は執筆者、研究代表者が行う。
- 公開可否に迷う資料があれば、GitHubに載せる前に確認する。
