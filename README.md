org-mobile-sync
===============

Automatically push and pull changes to/from MobileOrg

This just packages the following sections from the [MobileOrg FAQ](https://github.com/matburt/mobileorg-android/wiki/FAQ#wiki-How_do_I_get_orgmode_to_execute_orgmobilepush_automatically)

El-Get recipe:

```lisp
(:name org-mobile-sync
       :type git
       :url "https://github.com/steckerhalter/org-mobile-sync")
```

And then after `org-mode` has been loaded:

    (require 'org-mobile-sync)
