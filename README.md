# radipocket.github.io

らじぽけ（Radio Pocket）の組織のサイトです。**公式サイトは別のリポジトリ（radipocket/docs）で、https://radipocket.github.io/docs/ に出ています。**
このリポジトリに `docs` というフォルダを作らないでください（公式サイトの /docs/ と重なります）。

## 置いているもの

- `index.html`: トップ（/）を開くと公式サイト（/docs/）へ移る
- 短い転送用の URL（下の表）。開くとすぐ Google Play の、流入元の目印つきの URL へ移る
  - meta refresh（0秒）と `location.replace` の両方で移る。検索に出さない（noindex）。移らないとき用のリンクもある
  - 末尾の「/」があってもなくても開ける（GitHub Pages が /yt/s01 を /yt/s01/ へ移す）
  - 同じ表を `links.json` にも置いている（`upload_youtube.py` の確認は、公開ページの行き先を読んで目印を確かめる）
- `app-ads.txt`: AdMob の認定販売者の一覧（pub 番号はアプリの AdMob のアプリ ID と同じ）。Play のウェブサイトは https://radipocket.github.io/ にする
- `robots.txt`: 全部を許可し、公式サイトのサイトマップを書く
- `.nojekyll`: そのまま出す（Jekyll で組み立てない）

## 短い URL と行き先

| 短い URL | 行き先 |
|---|---|
| `https://radipocket.github.io/yt/long` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dlong` |
| `https://radipocket.github.io/yt/th` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dteaser_h` |
| `https://radipocket.github.io/yt/tv` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dteaser_v` |
| `https://radipocket.github.io/yt/s01` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort01` |
| `https://radipocket.github.io/yt/s02` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort02` |
| `https://radipocket.github.io/yt/s03` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort03` |
| `https://radipocket.github.io/yt/s04` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort04` |
| `https://radipocket.github.io/yt/s05` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort05` |
| `https://radipocket.github.io/yt/s06` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort06` |
| `https://radipocket.github.io/yt/s07` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort07` |
| `https://radipocket.github.io/yt/s08` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort08` |
| `https://radipocket.github.io/yt/s09` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort09` |
| `https://radipocket.github.io/yt/s10` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dyoutube%26utm_medium%3Dvideo%26utm_campaign%3Dshort10` |
| `https://radipocket.github.io/x` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dx%26utm_medium%3Dsocial%26utm_campaign%3Daruaru10` |
| `https://radipocket.github.io/ig` | `https://play.google.com/store/apps/details?id=ca.radipocket&referrer=utm_source%3Dinstagram%26utm_medium%3Dsocial%26utm_campaign%3Daruaru10` |

YouTube の目印（utm_campaign）: long・teaser_h・teaser_v・short01〜short10（RP-079）。X・Instagram はプロフィール用（RP-082）。2026-10-02 から、プロフィールの2本も出す先ごとの印（`utm_source=x`・`instagram`）と企画の印（`utm_campaign=aruaru10`）にした（RP-111）。

## 直し方

作り直すのは、らじぽけ本体の作業の手順（RP-082）の生成の道具です。手で直すときは、`links.json`・該当の `index.html`・この表の3か所をそろえてください。
main へ直接 push せず、PR で入れます。
