# dc-mf-treemap

桜千株式会社の MF クラウド会計 PL から生成する「お金のブロックパズル」standalone view。

- 公開先: https://jyajyamen13-eng.github.io/dc-mf-treemap/
- ビルド元: `cccbot/tools/mf-profit-treemap/build-standalone.py`
- 同期元: `cccbot/scripts/sync-mf-treemap.py`
- 自動更新: 毎日朝 8:30 JST (cccbot `JOBS.yaml: mf-treemap-rebuild`)

## 内容

- 全社合計 / 工事部 / 事業開発部 の 3 ビュー
- 売上 → 変動費 → 粗利 → 固定費 → 利益 のブロックパズル可視化
- AI 簡易分析コメント（ANTHROPIC_API_KEY 設定時は Claude API、未設定時はルールベース）

## 編集禁止

`index.html` は build script の出力で、直接編集しても次のビルドで上書きされる。
変更したい場合は cccbot 側の `tools/mf-profit-treemap/static/index.html` を編集する。
