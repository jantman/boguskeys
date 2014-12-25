boguskeys
=========

[![Project Status: Unsupported - The project has reached a stable, usable state but the author(s) have ceased all work on it. A new maintainer may be desired.](http://www.repostatus.org/badges/0.1.0/unsupported.svg)](http://www.repostatus.org/#unsupported)

GitHub's SSH key handling is awful. A key that GitHub knows about *anywhere*
can get SSH access. To do a read-only git clone over SSH (i.e. if you're cloning
a public repo and its submodules have git@github.com URLS), your user's SSH key
has to be known to GitHub *somewhere*, and it works. Try from a just-built dev VM,
and the submodule init fails because GitHub doesn't know about the key.

So, this repo exists just so I can set random dev VM's SSH keys as "deployment keys",
just to allow those random VMs to `git submodule update --init` third-party repos.

