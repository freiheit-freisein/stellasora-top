# 巡遊者ノート - Trekkers’ Notes（stella-tool.com のトップ）

ステラソラの非公式ツール集「巡遊者ノート」の入口のページ。

- `site/` … 公開するファイル（このフォルダだけを Cloudflare Pages に上げる）
- `tools/og.svg` → `node tools/make_og.mjs` で `site/og.png`（リンクのカード画像）を作る
- スクリーンショット（`site/img/*.webp`）は、公開中の計算ノート・素質ノートを画面なしの Chrome で開き、見せたい部分だけを2倍で切り出したもの

## 公開

```
../stellasora-site/node_modules/.bin/wrangler pages deploy site --project-name stellasora-top --branch main --commit-dirty=true
```

中身を変えたら `site/sitemap.xml` の lastmod も直す。
