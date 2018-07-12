# Vim kouza supplemental text

## Text Object Practice

Let's modify "^^^^" !
And undo with "u" !

### diw & daw / ciw & caw

The quick brown fox jumps over the lazy dog
          ^^^^^

The quick brown fox jumps over the lazy dog
          ^^^^^^

### di( & dw( / ci( & cw(

if (flag == true)
    ^^^^^^^^^^^^

if (flag == true)
   ^^^^^^^^^^^^^^

### di{ & da{ / ci{ & ca{

if (flag == true) {
    hoge = fuga
    ^^^^^^^^^^^
}


if (flag == true) {
    hoge = fuga   ^
    ^^^^^^^^^^^
}
^

### di" & da" / ci" & ca"

echo("hogefuga" + $num)
      ^^^^^^^^

echo("hogefuga" + $num)
     ^^^^^^^^^^

#### TIPS

|e|cho("hogefuga" + $num)
 ^
CURSOR

### di[ & da[ / ci[ & ca[

{"foo": [1, null, 12345], "baz": {"foo": [true, "bar"], "baz": "qux"}}
         ^^^^^^^^^^^^^^

{"foo": [1, null, 12345], "baz": {"foo": [true, "bar"], "baz": "qux"}}
        ^^^^^^^^^^^^^^^^

#### Review

{"foo": [1, null, 12345], "baz": {"foo": [true, "bar"], "baz": "qux"}}
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

{"foo": [1, null, 12345], "baz": {"foo": [true, "bar"], "baz": "qux"}}
                                  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

### dat & dit / cat & cit

<div id="hogefuga">
    <p>fizzbuzz</p>^
    ^^^^^^^^^^^^^^^^
</div>

<div id="hogefuga">
^^^^^^^^^^^^^^^^^^^^
    <p>fizzbuzz</p>
    ^^^^^^^^^^^^^^^^
</div>
^^^^^^

<div id="hogefuga">
    <p>fizzbuzz</p>
       ^^^^^^^^
</div>

<div id="hogefuga">
    <p>fizzbuzz</p>
    ^^^^^^^^^^^^^^^
</div>

## Plugin <surround.vim> Practice

### cs"' & ds"

"Hello World!"
^            ^

### ysiw] or ysw]

 Hello  World
^     ^

### ysiw<p> or ysw<p>

 Hello  World
^     ^

### v -> select from "H" to "o" -> S"

 "Hello  Wor"ld
^     ^
