
## Practice1

下の5コマンドを覚えて順番に実行して下さい

```
:e file1.txt
:e file2.txt
:e file3.txt
:ls
:1b
```

## Practice2

以下のコマンドを覚えて、 順番に実行し、 `Ctrl-^` を押して
オルタナティブバッファ(#)を行き来しながらanswerを埋めて下さい。

```
:e reference.txt
:e answer.txt
:ls
```

## Practice3

マッピングは定義してある前提です。
以下のコマンドをそのまま実行してみましょう。
このwindowは見えたままになるので、覚える必要はありません。

```
sv
sl
:e ../07vimrc
ss
:e file2.txt
sh
ss
sj
:e file1.txt
sk
```

うまくいけばこのwindowに戻ってきているはずです。

## Practice4
Practice3でやったように、 s + hjkl でウィンドウ間を移動できます。

07vimrcを開いているウィンドウまで移動し、
"Lesson07"で追加されたマッピング定義をコピー(yank)して、
このWindowまで戻ってきて、 下に貼り付けて下さい

++++++この間に++++++

+++++貼り付けて+++++

## Pracitce5
s + HJKL (大文字) で、 ウィンドウ自体を移動できます。

適当に動かしてみましょう


## Practice6
このWindow"以外"をCloseしましょう。
Closeは `:q` つまり普通に消します。
vim講座で入れたmappingを使いましょう。
`<Space>q`です。

