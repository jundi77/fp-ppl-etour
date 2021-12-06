# FP PPL ETOUR

Yang berada di repo ini adalah usaha untuk merapikan kode dari ETOUR, sumber asli kode ada di https://github.com/CoEST/TraceLab/tree/master/Main/Data/ANC-Data/eTour

regex
- ^/ \*\* jadi /**
- ^  \* / jadi "  */"
- ^\* / jadi "*/"
- \* /$ jadi "*/"
- `^/ /` jadi //
- ^\($ jadi {
- ($ jadi {
- ^\)$ jadi }
- ^\) $ jadi }
- TRY jadi try
- catch (.*)\($ jadi catch $1{
- ") catch" jadi } catch
- ^Private jadi private
- ^Public jadi public

ditata dengan jindent (https://ptolemy.berkeley.edu/java/jindent.htm)

```sh
for file in ./*
do
        jindent  $file
done
```