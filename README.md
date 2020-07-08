This edition of the book has been converted to LaTeX.
In order to build it, ensure you have a TeX distribution that contains
the `pdflatex` command. With that, you should be able to build the book
by running `make`, which will clone the OS itself and build the book
to `book.pdf` in the main directory.

# ビルド方法

プリプロセッサである lineref が，ファイル中の lineref コマンド（例:
`\lineref{kernel/proc.h:/^struct.context/}`）を見つけ，ソースコードを
参照して行番号を入力する．生成したコードは latex.out に入る．

カレントディレクトリに xv6-riscv-src という名前でソースコードのディレクトリ
が必要．以下のようにできる．

``` shell
% git clone https://github.com/mit-pdos/xv6-riscv.git xv6-riscv-src
```

# ビルドに関する変更点

日本語を扱うために，pdflatex から platex に変更．

