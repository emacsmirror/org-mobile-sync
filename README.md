org-mobile-sync
===============

Automatically push and pull changes to/from [MobileOrg](http://orgmode.org/manual/MobileOrg.html).

Some of the code has been taken from the [MobileOrg FAQ](https://github.com/matburt/mobileorg-android/wiki/FAQ).

I added support for inotify so that changes of the `org-mobile-capture-file` are detected immediately and trigger a `org-mobile-pull`.

**Emacs 24.3.50 with `file-notify-support` is required for the mode to work.**

El-Get recipe:

```lisp
(:name org-mobile-sync
       :type git
       :url "https://github.com/steckerhalter/org-mobile-sync")
```

And then after `org-mode` has been loaded:

    (require 'org-mobile-sync)
    (org-mobile-sync-mode 1)
