# 画像のデジタル化君

正方形のキャンバスに絵を描き、解像度と色の表し方による見た目・データ量の変化を比べる学習用アプリです。

## 使い方

`index.html` または `img_digital_kun.html` をブラウザで開いてください。HTML単体で動き、外部ライブラリ・外部送信・アクセス解析はありません。保存後はオフラインで利用できます。

- マウス・タッチ・タッチペンで描画、元に戻す、全消去
- ペンのカラーコードとRGB値を表示
- 解像度：8、16、32、64、128、256画素の正方形
- モノクロ（白黒2値：1 bit）、グレースケール（256階調：8 bit）、カラー（RGB各256階調：24 bit）
- 元画像と加工後画像、画素数、理論上のデータ量を比較

データ量は「幅 × 高さ × 1画素のビット数 ÷ 8」です。ファイル形式のヘッダー、圧縮、透過情報などは含みません。内部のCanvasが使うメモリ量とも異なります。

## ダウンロード

`download.html` は確認付きのダウンロードページです。アクセスしただけでは保存を開始しません。`img_digital_kun.html` は配布用の同内容のHTMLです。アプリ内のダウンロードでも確認後にHTMLを保存できます（描いた絵の保存機能ではありません）。

## GitHub Pages

Settings → Pages → Build and deployment → Deploy from a branch → main / (root) → Save。

公開後の利用URL：https://ken-tak-steam.github.io/img_digital_kun/

ダウンロードページ：https://ken-tak-steam.github.io/img_digital_kun/download.html

Googleサイトには公開後の利用URLを埋め込めます。

## 対応・確認状況

Chrome・Edge・Safariの標準Web APIを使用しています。計算・画像変換・描画・元に戻す処理はCanvas実行環境で確認しました。実ブラウザの操作およびiPad・Apple Pencilでの実機確認は未実施です。

## ライセンス

[LICENSE](./LICENSE) を参照してください。著作者表示付き・非商用での使用、改変、再配布を認めます。学校教育、講習会、研修会での教材利用は有料・無料を問いません。
