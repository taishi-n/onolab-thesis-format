# 小野研究室 学位論文フォーマット
[サンプル](./build/20XX_Thesis_Example.pdf)

## 動作環境
### Windows
Windowsでの動作はまだ確認できていません，ごめんなさい
検証したらちゃんとまとめます
次などを参考にしてみてください
- https://note.com/ojk/n/n6c8f6a30b67a
- http://www.slis.tsukuba.ac.jp/~fujisawa.makoto.fu/cgi-bin/wiki/index.php?TexLive%2BAtom

### Linux/macOS
#### TeX Live
- https://texwiki.texjp.org/?TeX%20Live%2FMac#texlive-install-pacman
```
brew install mactex
```

#### コンパイル方法
```
latexmk -r latexmkrc
```

## ファイル構成
- `bib/`: bibtexファイル
- `build/`: 出力結果
- `fig/`: 図
- `sections/`: 節ごとのTeXファイル
- `20XX_Thesis_Example.tex`: 原稿本体
- `README.md`
- `latexmkrc`: latexmk設定ファイル
- `onolabthesis.sty`: 本テンプレートスタイルファイル
