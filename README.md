# 特典会タイマー 公開ページ

サポート・プライバシーポリシー・利用規約をGitHub Pagesで公開する静的サイトです。サーバー、npm、独自ドメインは不要です。公開前に運営者の表記と規約を確認してください。

## ブラウザで公開する

1. GitHubにログインし、新しいリポジトリを作ります。名前の例は `tokutenkai-timer-support`。GitHub Freeで公開する場合は **Public**、**Add README** をオンにします。
2. リポジトリの **Add file → Upload files** を選びます。このフォルダの `index.html`・`privacy.html`・`terms.html`・`styles.css`・`app-icon.png` の **5ファイルを直接アップロード**し、**Commit changes** を押します。ZIPやフォルダを丸ごとアップロードせず、リポジトリの一番上に `index.html` が見える状態にします。このREADMEで作成時のREADMEを置き換えても構いません。
3. **Settings → Pages** で **Source: Deploy from a branch**、**Branch: main**、フォルダ **/(root)** を選び、**Save** を押します。標準ブランチをmain以外にした場合は、アップロード先のブランチを選びます。
4. 公開処理が終わったら、同じ画面に表示される **Visit site** で開きます。反映に最大10分ほどかかる場合があります。
5. ログアウトしたブラウザでもサポート・プライバシー・利用規約の3ページを開けることを確認します。CSSとアイコンは相対パスなので、リポジトリ名を変えても動きます。

`.nojekyll` はJekyllを使わず静的ファイルを配信するための空ファイルです。Git操作やGitHub Desktopで投稿する場合は含めてください。ブラウザで上記5ファイルだけをアップロードする方法でも、このサイトのHTML・CSS・PNGを公開できます。

## 公開後にアプリへ登録する

公開画面に表示された実際のURLを使います。リポジトリの `github.com/...` URLは、公開ページのURLではありません。

- サポートURL：公開したサイトのトップ
- プライバシーURL：同じサイトの `privacy.html`
- 補足利用規約URL：同じサイトの `terms.html`

アプリの `特典会タイマー/Services/AppLegal.swift` の `supportURL`・`privacyPolicyURL`・`supplementalTermsURL` を、この実URLに設定します。App Store Connectにも同じサポート・プライバシーURLを登録します。現在はGitHubへの投稿・サイト公開がまだ完了していないため、アプリ側はnilのままです。仮URLで購入を有効にしないでください。

## 文書を更新するとき

HTMLの文書は、アプリ内 `Resources/PrivacyPolicy.md`・`Resources/TermsOfUse.md` と同じ内容を保持してください。今の月額150円・年額1,000円は予定料金です。App Store Connectで料金が確定した後、アプリ内文書・公開ページ・掲載文を一緒に更新してください。サイトの変更をCommitすると、GitHub Pagesに反映されます。

お問い合わせ：poran.support@proton.me

GitHub公式手順：[GitHub Pagesサイトの作成](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)、[公開元の設定](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
