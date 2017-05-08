DotEmacs
========

This repository contains my personal Emacs configuration.

Have fun tinkering : j

What the .el
============

If you are wondering where has gone all of the Lisp, fear not, for it is
automagically tangled from an Org file into a fresh Lisp file with the help of the
all powerful `org` package. This is called literate programming.

Head over to the actual configuration: [dotemacs.org][self.dotemacs].

Screenshots
===========

My Emacs configuration is a living mixture that I edit on a daily basis. As such, the
following screenshots might not reflect exactly what is on `:master`.

- [Helm][screenshots.helm]

More coming *soon* :tm:

Installation
============

I primarily use Emacs on OS X, but I trust your *google-fu* to find the equivalent for
the following commands to run on your setup.

Emacs
-----

I use [Emacs Plus][github.homebrew-emacs-plus]. The configuration files *should* work with
any build nonetheless. In any case, install Emacs 24 or above.

``` sh
brew tap d12frosted/emacs-plus
brew install emacs-plus --with-no-title-bars --without-spacemacs-icon
git clone https://github.com/angrybacon/dotemacs.git ~/.emacs.d/
```

Ag
--

My Helm setup uses `ag` instead of `grep` to lookup files.

```sh
brew install the_silver_searcher
```

Flycheck
--------

I use [Flycheck][github.flycheck] as linter framework to display syntax warnings and
errors whithin each buffer.

```sh
pip install flake8                                   # Python
gem install scss_lint scss_lint_reporter_checkstyle  # SCSS
npm install -g eslint                                # JavaScript
```

Material Design Icons
---------------------

There are special characters in the mode-line. Install [`mdi`][mdi].

[mdi]: https://materialdesignicons.com
[github.flycheck]: https://github.com/flycheck/flycheck
[github.homebrew-emacs-plus]: https://github.com/d12frosted/homebrew-emacs-plus
[screenshots.helm]: https://drive.google.com/open?id=0BwTSOByd3qSFMmZqVHBpTlk2Q1E
[self.dotemacs]: ./dotemacs.org
