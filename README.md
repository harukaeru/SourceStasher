# [WIP]SourceStasher

This is WIP. No able to use.

## Specification

*johnny.txt*
```
Hello
I am Johnny.
I am a man.
```
　  ↓
```sh
$ stasher johnny-to-kaeru
```
　  ↓


*kaeru.txt*
```
Hello
I am Kaeru.
I am a woman.
```
　　↓
　　
Editing

*kaeru.txt*
```
Hello
I am Kaeru.
I like an apple.
```
　　↓
```sh
$ stasher --destash johnny-to-kaeru --dry_run
```
```
Hello
# I am Johnny.
#-I am a man.  <-- Will be deleted.
# I like an apple
```

　　↓
　　
```sh
$ stasher --destash johnny-to-kaeru
```
*johnny.txt*
```
Hello
I am Johnny.
I like an apple
```
