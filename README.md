vimanage
========

Another opinionated Vim plugin manager for [pathogen][] users.

It presupposes that:

* you use pathogen with default bundle directory (`~/.vim/bundle`)
* you use git to install plugins

How to use
----------

Install a plugin from git repository url:

    vimanage -i plugin-git-url

Deletes a plugin:

    vimanage -d plugin-directory

Lists installed plugins:

    vimanage -l

Save installed plugins to file:

    vimanage -l > plugins.txt

This works the same way python's `pip freeze > requirements.txt` works.

Install plugins from file (one git repository per line):

    vimanage -i plugins.txt

Just like `pip install -r requirements.txt`.

Help:

    vimanage -h

How to install
--------------

Copy `bin/vimanage` script to your path.

License
-------

MIT licensed.

[pathogen]: https://github.com/tpope/vim-pathogen
