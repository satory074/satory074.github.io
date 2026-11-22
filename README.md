# satory074.github.io

GitHub Pages の「ユーザーサイト」。中身は 3 つだけ:

- `robots.txt` — `satory074.github.io/<repo>/` で公開している各アプリのサイトマップを `Sitemap:` 行で並べる。
  github.io のプロジェクトサイトでは、検索エンジンが読むのはドメイン直下のこの robots.txt だけ
  (各アプリの中に置いた robots.txt は読まれない)
- `index.html` — noindex。アプリ一覧 (satory074.com/apps/) へのリンクだけ
- `google<token>.html` — Google Search Console の URL プレフィックスプロパティ `https://satory074.github.io/` の所有確認用

**独自ドメイン (CNAME) は付けない**。付けると全アプリの URL がそのドメインの下に移り、端末保存データ (localStorage) が消える。
アプリと同じ名前のフォルダをここに作らない (アプリのパスと衝突する)。

新しいアプリを掲載したら、そのサイトマップを `robots.txt` に足す (basecamp/docs/app-backlink.md のチェックリスト)。
AI クローラーも含めて全許可 (2026-11-21 の判断)。
