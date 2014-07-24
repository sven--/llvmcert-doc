### On Coq ###

Coq is an interactive theorem prover, in which you can define a
function, state a property on the function, and prove the property.

## Installation ##

# Coq #

* Download Coq [here](http://coq.inria.fr/download) and install it.

  + For OS X, you may have to properly set path variable. add the
    following in `~/.bashrc`:
    ```
    export PATH=/Applications/CoqIdE_8.4pl4.app/Resources/bin/:$PATH
    ```
    The path may be updated; be cautious before blindly adding the line.

* Test by `coqc -v` in the command line.

# Git #

Download [here](http://git-scm.com/downloads).

# Emacs #

Currently, Emacs is practically the only editor that supports
interactive theorem proving with Coq.

* Install Emacs.

  + For OS X, download [here](http://emacsformacosx.com/).

* Download `.emacs`.

  + `git clone https://github.com/lunaticas/configurations.git`

  + `cp configurations/.emacs* ~`

  + You may have to edit `.emacs`. Particularly, if necessary, remove
    TeX part.

* Configure Emacs.

  + Run Emacs.

  + Type `M-x`, then `list-packages`. Install any package you
    like. Note that `M-` means alt, and `C-` means ctrl.

  + Rerun Emacs. It will ask you to install packages. Repeat type `y`.

* Read Tutorial by typing `C-h t`.

# Study Software Foundations #

* Download [here](http://www.cis.upenn.edu/~bcpierce/sf/current/index.html).

* Make a Git repository for it.

* Upload to [Github](https://github.com/).

* Open `.v` files in Emacs, and interactively use Coq. Here are some
  useful commands; try them.

  + `C-c C-n`

  + `C-c C-p`

  + `C-c C-Enter`

  + `C-c C-b`

  + `C-c C-x`

  + `C-c C-a C-c`

  + `C-c C-a C-p`

  + `C-c C-a C-a`

  + Combination that begins with `C-c`

* Add mentors to your Github repository, and if you have a question,
  post an issue in Github. Mentors will help.
