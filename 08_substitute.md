# Vim kouza supplemental text for Lesson 08

## 1. Substitution in one line

1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
^
Put cursor here and type the command below and hit Enter.
Repeat this **4 times!**

`:s/XXX/Changed!`


## 2. Substitution in one line. Repeat with "&" key

1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
^
Put cursor here and type the command below and hit Enter.
**AND TYPE "&" 3 TIMES**

`:s/XXX/Changed!`


## 3. Substitution in one line with "i" option (ignorecase)

1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
^
Put cursor here and type the command below **5 times!**
NOTE: "&" doesn't work :(

`:s/xxx/Changed!/i`


## 4. Substitution in one line with "g" option (global)

1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
^
Put cursor here and type the command below!

`:s/XXX/Changed!/g`


## 5. Substitution in one line with "ig" option (ignorecase and global)

1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
^
Put cursor here and type the command below!

`:s/XXX/Changed!/ig`

## 6. Substitution in one line with "igc" option (ignorecase and global and confirm)

1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6. Xxx, 7:YYY, 8:XXX
^
Put cursor here and type the command below!

`:s/XXX/Changed!/igc`


## 7. Substitution in multiple lines

1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX
1: XXX, 2: YYY, 3: XXX, 4: XXX, 5: ZZZ, 6: Xxx, 7:YYY, 8:XXX

Select from 1st to 3rd lines with <S-v> and type the command below!

`:s/XXX/Changed!/g`


## 8. Substitution across the buffer

Type the command below! "%" means "all contents in this buffer"

`:%s/Changed/YEEEEEEAH/g`
