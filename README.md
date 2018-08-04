# Steps to reproduce

```
npx shadow-cljs node-repl
```

```
[0:0]~cljs.user=> (require 'foo.bar :reload)
```

```
[0:0]~cljs.user=> (foo.bar/baz)
Baz!
nil
```

Edit file `bar.cljs` to print something else instead.

```
[0:0]~cljs.user=> (require 'foo.bar :reload)
nil
[0:0]~cljs.user=> (foo.bar/baz)
Baz!
nil
```
