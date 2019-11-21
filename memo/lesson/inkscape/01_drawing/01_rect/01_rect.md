# 描画する

* 矩形（長方形・正方形）

## 矩形（長方形・正方形）

1. ツールボックスから「矩形」をクリックする
1. D&Dする

　`Ctrl`を押下しながらD&Dすれば整数比になる。

## 変形

1. ツールボックスから「選択」をクリックする
1. 頂点をクリックする
1. D&Dする

　なお、変形方法は以下の2つ。対象をクリックすると周辺のアイコン表示が変わるので見分けられる。

* 拡大・縮小
* 回転

　また、`Ctrl`を押下しながらD&Dすれば整数比になる。たとえばキッチリ90度回転させることなどができる。15度間隔だった。

## 基礎

### ツールボックスを表示する

　もしツールボックスが非表示なら表示する。

1. メニュー
1. 表示 `Alt+V`
1. 表示/非表示 `O`
1. ツールボックス `T`

### SVGに出力する

1. メニュー `Alt+F`
1. 名前をつけて保存 `A` or `Shift+Ctrl+S`
1. パスを入力する
1. 拡張子を`svg`にする

#### SVGを編集する

　テキストエディタで開く。

　以下のような構造になっていた。`layer`の中に`rect`が含まれている。

```svg
  <g
     inkscape:groupmode="layer"
     id="layer2"
     inkscape:label="レイヤー 2">
    <rect
       style="fill:#000000;stroke-width:0.81809396"
       id="rect17"
       width="170.16354"
       height="170.16354"
       x="-129.51559"
       y="175.70349"
       transform="matrix(0.86433446,-0.50291743,0.86433446,0.50291743,0,0)" />
  </g>
```

　`circle`の位置や半径を調整してやればキレイに整形できる。

属性|意味
----|----
`cx`|X座標位置
`cy`|Y座標位置
`r`|半径

#### SVGを圧縮する

　Webサービスを使う。

* https://jakearchibald.github.io/svgomg/

#### デフォルト設定にする

　inkscape起動時にデフォルトで円が書かれたレイヤーが欲しいとき。

　以下ファイルに内容を上書きする。

```sh
/usr/share/inkscape/templates/default.ja.svg
```

　またはテンプレとする。読取専用SVGファイルとして保存し、それを開いて編集し、名前をつけて保存する。

# 黄金比

* [黄金比](https://ja.wikipedia.org/wiki/%E9%BB%84%E9%87%91%E6%AF%94)
* [黄金長方形](https://ja.wikipedia.org/wiki/%E9%BB%84%E9%87%91%E9%95%B7%E6%96%B9%E5%BD%A2)

　golden rato
　golden rectangle svg

* https://commons.wikimedia.org/wiki/File:Fibonacci_spiral.svg
* https://commons.wikimedia.org/wiki/File:Fibonacci_spiral_34.svg
* https://dribbble.com/shots/6037380-Golden-Ratio-illustrator-Template-AI-SVG

種類|概算|少数|式
----|----|----|--
黄金比|5:8|1:1.618|1:(1+√5)/2
白銀比|5:12|1:2.414|1:1+√2
白銀比|5:7|1:1.414|1:√2

