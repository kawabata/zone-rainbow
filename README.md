Zone out with rainbow
=====================

Zone out with rainbow. This code is inspired by <https://gist.github.com/mrkuc/7121179>.

It can be directly invoked by `M-x zone-rainbow`.

It can be set as a single zone program by the following.

``` common-lisp
  (setq zone-programs '(zone-pgm-rainbow))
```

Or, it can be added to zone program list as follows.

``` common-lisp
  (callf2 mapcar 'identity zone-programs) ; in case `zone-programs' is vector.
  (add-to-list 'zone-programs 'zone-pgm-rainbow)
```
