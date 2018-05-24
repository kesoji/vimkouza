
## Practice1

下の4コマンドを覚えて順番に実行して下さい

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
" Lesson07
" Window operation
nnoremap s <Nop>
nnoremap ss :<C-u>split<CR>
nnoremap sv :<C-u>vsplit<CR>
" Move around window
nnoremap sj <C-w>j
nnoremap sk <C-w>k
nnoremap sl <C-w>l
nnoremap sh <C-w>h
" Move window
nnoremap sJ <C-w>J
nnoremap sK <C-w>K
nnoremap sL <C-w>L
nnoremap sH <C-w>H

" Lesson07
" quickfix and vim[grep
nnoremap <C-n> :cnext<CR>
nnoremap <C-p> :cprevious<CR>
+++++貼り付けて+++++



## Pracitce5
s + HJKL (大文字) で、 ウィンドウ自体を移動できます。

適当に動かしてみましょう


## Practice6
このWindow"以外"をCloseしましょう。
Closeは `:q` つまり普通に消します。
vim講座で入れたmappingを使いましょう。
`<Space>q`です。

## Practice7

