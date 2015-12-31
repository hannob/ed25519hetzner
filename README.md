# ed25519hetzner
Script to scan OpenSSH host key and known_hosts files for shared keys from server hoster Hetzner

usage
=====

 `./ed25519hetzner [files]`

If script runs with user rights and no files are given the script checks
the user's known_hosts and if available the system's ed25519 key.

If script runs as root it checks the root's, all user's known_hosts and
the system's ed25519 key.

background
==========

Between April 2015 and December 2015 Hetzner preinstallation images contained
a shared Ed25519 key.

* http://wiki.hetzner.de/index.php/Ed25519/en
* http://blogs.intevation.de/thomas/hetzner-duplicate-ed25519-ssh-host-keys/
