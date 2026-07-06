# Gyokuto株式会社 BPOサービスサイト

Gyokuto株式会社のBPOサービスサイトです。HTML、CSS、JavaScriptのみで構成しているため、GitHub Pagesでそのまま公開できます。

## ファイル構成

- `index.html`：トップページ（`https://bpo.gyokuto-inc.com/`）
- `home.html`：ホームページ（`https://bpo.gyokuto-inc.com/home.html`）
- `services.html`：サービス内容
- `pricing.html`：料金・見積
- `flow.html`：導入の流れ
- `faq.html`：よくある質問
- `company.html`：会社概要
- `contact.html`：お問い合わせ
- `estimate.html`：お見積り
- `privacy.html`：プライバシーポリシー
- `thanks.html`：送信完了ページ
- `sitemap.xml`：検索エンジン向けサイトマップ
- `robots.txt`：クロール方針とサイトマップURL
- `assets/css/styles.css`：共通スタイル
- `assets/js/main.js`：ナビゲーション
- `assets/images/hero-workspace.png`：トップページ画像

## GitHub Pagesでの公開方法

1. このフォルダの内容をGitHubリポジトリにアップロードします。
2. GitHubのリポジトリ画面で `Settings` を開きます。
3. `Pages` を選択します。
4. `Build and deployment` の `Source` で `Deploy from a branch` を選択します。
5. `Branch` で公開するブランチと `/root` を選択し、保存します。
6. 表示された公開URLでサイトを確認します。

BPOサービスサイトの想定URLは `https://bpo.gyokuto-inc.com/` です。GitHub Pagesの `Custom domain` に `bpo.gyokuto-inc.com` を設定し、DNS側でGitHub Pages向けのレコードを設定してください。

ローカルで表示確認する場合は、このフォルダの `index.html` をブラウザで開いてください。

ページURLの想定：

- トップ：`https://bpo.gyokuto-inc.com/`
- ホーム：`https://bpo.gyokuto-inc.com/home.html`
- サービス内容：`https://bpo.gyokuto-inc.com/services.html`
- 料金・見積：`https://bpo.gyokuto-inc.com/pricing.html`
- 導入の流れ：`https://bpo.gyokuto-inc.com/flow.html`
- FAQ：`https://bpo.gyokuto-inc.com/faq.html`
- お問い合わせ：`https://bpo.gyokuto-inc.com/contact.html`
- お見積り：`https://bpo.gyokuto-inc.com/estimate.html`

## Search Consoleでの初期設定

Google Search Consoleの `サイトマップ` で、次のURLを送信してください。

```text
https://bpo.gyokuto-inc.com/sitemap.xml
```

## フォーム送信について

`contact.html` と `estimate.html` のフォームは、静的サイトでも送信できるように外部フォーム送信サービスへPOSTする構成です。

現在の送信先：

```html
https://formsubmit.co/customer-support@gyokuto-inc.com
```

初回送信時に、送信先メールアドレス側で有効化が必要になる場合があります。別のフォームサービスを利用する場合は、各フォームの `action` を差し替えてください。
