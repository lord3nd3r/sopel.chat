sopel.chat
==========

Website for [Sopel](https://github.com/sopel-irc/sopel), deployed at https://sopel.chat

Made for use with [jekyll](https://jekyllrb.com/). It's not hosted on GitHub
Pages, primarily so that we can have a more complex build process. (The [build
script](netlify-build.sh) calls some extra scripts to auto-generate some
things based on a specific version of Sopel's code.)


Working with automatically generated pages
------------------------------------------

See [UPDATING.md](UPDATING.md).


Sopel source submodule
---------------------

This repo uses a git submodule at `_sopel/` containing the Sopel source tree,
which is used by the build scripts to generate parts of the site.

Clone with submodules:

```bash
git clone --recurse-submodules https://github.com/lord3nd3r/sopel.chat
```

Or, if you already cloned the repo:

```bash
git submodule update --init --recursive
```
