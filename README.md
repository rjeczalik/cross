cross
=====

A simple bash script for enhancing current `$GOROOT`/pkg with official packages for all the major platforms. Using binary packages from golang.org/dl, which are compiled on a target os and architecture, does not have the same `CGO` restrictions as using crosscompiled packages.

*Installation*

```bash
~/bin $ wget -q https://raw.githubusercontent.com/rjeczalik/cross/master/gocross -O - \
| tee ~/bin/gocross | sha1sum - | cut -d' ' -f1 \
| xargs -i test  "{}" = "5910b55cc3046485c58337965ba8224801eece47" || rm -v ~/bin/gocross \
&& chmod +x ~/bin/gocross
```

*Pic or it didn't happen*

![gocross](http://i.imgur.com/uWs17Db.gif "gocross")
