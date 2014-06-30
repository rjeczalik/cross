cross
=====

A simple bash script for enhancing current `$GOROOT`/pkg with official packages for all major platforms. Using binary packages, compiled on the target os and architecture, does not have the same `CGO` restrictions as using crosscompiled packages.

*Installation*

```bash
~ $ wget -q https://raw.githubusercontent.com/rjeczalik/cross/master/gocross -O - | tee ~/bin/gocross | md5sum - | cut -d' ' -f1 | xargs -i test  "{}" = "9d79c278c11146653c4e832caf5df281" || rm -v ~/bin/gocross
```

*Pic or it didn't happen*

![gocross](http://i.imgur.com/uWs17Db.gif "gocross")
