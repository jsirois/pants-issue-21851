This is a minimal repo setup that tries to repro the issue in 
https://github.com/pantsbuild/pants/issues/21851.

A critical aspect of that issue is the presence of CPython 3.10.16+ in
Pants Python search path, which should be acheived by installing
3.10-dev with pyenv. You should see:
```
:; pyenv versions | grep 3.10-dev
  3.10-dev
```
