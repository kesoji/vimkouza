# Vim kouza supplemental text

## Text Object Practice

Let's modify "^^^^" !

### daw & diw / caw & ciw

The quick brown fox jumps over the lazy dog
          ^^^^^

The quick brown fox jumps over the lazy dog
          ^^^^^^

### da( & di( / ca( & ci(

if (flag == true)
    ^^^^^^^^^^^^

if (flag == true)
   ^^^^^^^^^^^^^^

### da{ & di{ / ca{ & ci{

if (flag == true) {
    hoge = fuga
    ^^^^^^^^^^^
}


if (flag == true) {
    hoge = fuga   ^
    ^^^^^^^^^^^
}
^

### ca" & ci" / ca" & ci"

echo("hogefuga" + $num)
      ^^^^^^^^

echo("hogefuga" + $num)
     ^^^^^^^^^^


#### TIPS

|e|cho("hogefuga" + $num)
 ^
CURSOR

### cat & cit / cat & cit

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

### ysiw]

 Hello  World
^     ^


### ysiw<p>

 Hello  World
^     ^

### v -> select from "H" to "o" -> S"


 Hello  World
^     ^
