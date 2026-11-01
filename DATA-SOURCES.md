# データソースと利用条件

本リポジトリは [Orbis](https://orbis-beta.vercel.app)（`sg55555/orbis`・個人運営・非商用）が
GitHub Actions で収集・整形した公開データのスナップショットを配布します。
JSON の構造は MIT（同梱 `LICENSE`）。**各データの権利は下表の上流に帰属し、
再利用はそれぞれの条件に従ってください。**

| 層 / ファイル | 上流 | 条件・帰属 |
|---|---|---|
| `quakes.json`（地震） | USGS Earthquake Hazards Program | 米国政府の著作物＝パブリックドメイン |
| `flights.json`（航空） | OpenSky Network | OpenSky の利用規約（非商用の研究利用） |
| `conflict.json` / `protests.json`（紛争・抗議） | The GDELT Project | GDELT の利用規約（出典表示・再配布可） |
| `ships.json`（船舶） | AISstream.io | AISstream の利用規約 |
| `news.json`（ニュース） | 各媒体の公開 RSS（見出し・要約・リンク） | 見出しと要約は **AI による日本語化**。本文は配布せず、原記事へリンクする。著作権は各媒体 |
| `sst.json`（海水温） | Open-Meteo Marine API | CC BY 4.0 — © Open-Meteo |
| `airtemp.json`（気温） | Open-Meteo API | CC BY 4.0 — © Open-Meteo |
| `firms.json`（山火事） | NASA FIRMS (MODIS / VIIRS) | NASA の公開データ。FIRMS の利用条件に従う |
| `briefing.json` / `instability.json` / `forecast.json`（AI 3 層） | 上記各層から Claude が合成 | **AI 生成物**（要約・推定）。誤りを含みうる。元データの条件が継承される |
| `profiles/*.json.gz`（地域プロフィール） | Wikipedia (ja) を AI が要約・再構成／Wikidata | 本文＝**CC BY-SA 4.0**（記事名を明示・再配布は同一ライセンス）。Wikidata プロパティ＝CC0 |
| `admin1/*.geojson.gz`・`admin1_bbox.json`（行政界） | Natural Earth | パブリックドメイン |
| 地図タイル（本リポには含まない） | OpenFreeMap / OpenMapTiles / OpenStreetMap contributors | ODbL — © OpenStreetMap contributors |

## 免責

- 収集は無保証・ベストエフォートです。欠測・遅延・誤りがありえます。
- 安全・投資・避難などの判断に用いないでください。
- 問い合わせ・削除依頼は GitHub Issues（<https://github.com/sg55555/orbis/issues>）へ。
