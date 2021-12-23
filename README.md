vimanage
========

Another opinionated Vim plugin manager.

It presupposes that:

* you use Vim 8 or above with native package manager
* you use git to install plugins

How to use
----------

**Install a plugin from git repository url:**

    vimanage add plugin-git-url

**Delete a plugin:**

    vimanage remove plugin-directory

**List installed plugins:**

    vimanage list

**Save installed plugins to a file:**

    vimanage list > plugins.txt

This works the same way python's `pip freeze > requirements.txt` works.

**Install plugins from file (one git repository per line):**

    vimanage add plugins.txt

Just like `pip install -r requirements.txt`.

**Help:**

    vimanage help

It can be used to install NeoVim packages as well by using
`VIMANAGE_ROOT` environment varibale, like this:

    VIMANAGE_ROOT=~/.local/share/nvim/site/pack vimanage add <plugin-url>


How to install
--------------

Copy `bin/vimanage` script to your path.

License
-------

MIT licensed.
