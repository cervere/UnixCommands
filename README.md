# UnixCommands

### Rename all the files in a folder according to a regex :

```
re@in:~$ ll
drwxrwxr-x  2 xyz xyz 4096 déc.  12 17:18 "Foo Bar" <foo.bar@etu.u-abc.fr>; /

re@in:~$ rename 's/^"(.*)" \<(.*)\>(.*)/$1_$2/g' *

re@in:~$ ll
drwxrwxr-x  2 xyz xyz 4096 déc.  12 17:18 Foo Bar_foo.bar@etu.u-abc.fr/
```

### Ocaml Tuareg mode in Emacs
https://howtos.gattaz.net/2015/09/14/install-ocaml-and-the-tuareg-mode-on-ubuntu-14-04/

### Copy every file in all directories
```
for f in ./*bordeaux.fr/*.ml; do cp "$f" "$(dirname "$f")/test.ml"; done
``` 
