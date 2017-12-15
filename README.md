# UnixCommands

### Rename all the files in a folder according to a regex :

```
re@in:~$ ll
drwxrwxr-x  2 xyz xyz 4096 déc.  12 17:18 "Foo Bar" <foo.bar@etu.u-abc.fr>; /

re@in:~$ rename 's/^"(.*)" \<(.*)\>(.*)/$1_$2/g' *

re@in:~$ ll
drwxrwxr-x  2 xyz xyz 4096 déc.  12 17:18 Foo Bar_foo.bar@etu.u-abc.fr/
```

