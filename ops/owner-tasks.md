# オーナーの作業リスト

終わったら [x] にするか、Claude に「○番終わった」と伝えてください。パスワードやトークンはチャットに貼らないでください。

## 共通の注意（匿名性）
- 作業は**ブラウザの別プロファイル**（Chrome なら「TaneBako」プロファイル）で行うと、個人アカウントとの取り違えや自動ログイン連携を防げます。
- 表示名・プロフィール画像・自己紹介に、本名・勤務先・地域を入れない。
- 個人のGmailを「再設定用メール」にしない（電話番号はGoogleの仕組み上必要なので、個人の番号でかまいません。公開はされません）。

## 1. TaneBako 用 Gmail を作る（2026-11-15 完了: tanebako.lab@gmail.com）
- [ ] 別プロファイルで Google アカウントを新規作成（名前「TaneBako」、アドレス例: `tanebako.xxx@gmail.com`）
- [ ] 2段階認証をオンにする
- [ ] ログイン情報は **個人の 1Password 保管庫** に保存（AI-Automation には入れない）
- [ ] 作ったアドレスを Claude に伝える（アドレスは秘密ではないので伝えてOK。台帳に書きます）

## 2. TaneBako 用 GitHub を作る（2026-11-15 完了: tanebakolab-glitch、push 設定済み）
- [ ] 上の Gmail で GitHub に登録（ユーザー名例: `tanebako`。取られていれば `tanebako-lab` など）
- [ ] 2段階認証をオンにする（ログイン情報は個人の保管庫へ）
- [ ] Settings → Emails で
  - [ ] 「Keep my email addresses private」をオン
  - [ ] 「Block command line pushes that expose my email」をオン
  - [ ] 表示される `数字+ユーザー名@users.noreply.github.com` を Claude に伝える（コミットの作者に使います）
- [ ] private リポジトリ `tanebako` を **空で** 作る（README・.gitignore・ライセンスは付けない）
- [ ] Fine-grained personal access token を作る
  - Repository access: Only select repositories → `tanebako` だけ
  - Permissions: Contents = Read and write（他は触らない）
  - 有効期限: 1年（期限前に作り直す）
- [ ] トークンを 1Password **`AI-Automation`** に項目 `tanebako-github`（フィールド `credential`）で保存
- [ ] Claude に「GitHub できた、ユーザー名は ○○」と伝える → push の設定をします

## 3. 以降（準備期間中に案内します）
- X・note のアカウント開設（承認制。命名案は Claude が出します）
- YouTube・TikTok の名前の確保
