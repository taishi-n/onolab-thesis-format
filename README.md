# 小野研究室 学位論文フォーマット
[サンプル](./build/20XX_Thesis_Example.pdf)

## コンパイル方法
### Windows
- TeX Works
  1. `20XX_Thesis_Example.tex` を開く
  2. エンジンを `upLaTeX(ptex2pdf)` に指定する
  3. タイプセットする
- VSCode
  1. LaTeX の設定をする (参考: https://note.com/ojk/n/n6c8f6a30b67a)
  2. `20XX_Thesis_Example.tex` を開く
  3. タイプセットする
- Atom + LaTeX
  1. LaTeX の設定をする (参考: http://www.slis.tsukuba.ac.jp/~fujisawa.makoto.fu/cgi-bin/wiki/index.php?TexLive%2BAtom)
  2. `20XX_Thesis_Example.tex` を開く
  3. タイプセットする

#### 漢字やカタカナが表示されない場合
`onolabthesis.sty` の28行目
```
\usepackage[expert,deluxe,jis2004,uplatex]{otf}
```
をコメントアウトしてください．
原因は調査中です．

### Linux/macOS
ターミナルで次を実行
```
latexmk -r latexmkrc
```

上に書いた VSCode, Atom も Windows の場合と同様にできます

## ファイル構成
- `bib/`: bibtexファイル
- `build/`: 出力結果
- `fig/`: 図
- `sections/`: 節ごとのTeXファイル
- `20XX_Thesis_Example.tex`: 原稿本体
- `README.md`
- `latexmkrc`: latexmk設定ファイル
- `onolabthesis.sty`: 本テンプレートスタイルファイル
