1. `gpg --full-generate-key` Create a key by using an algorithm.
2. Get generated key by executing: `gpg --list-keys`
3. Set the key here `git config --global user.signingkey <Key from your list>`
4. `git config --global gpg.program /usr/local/bin/gpg`
5. `git config --global commit.gpgsign true`
6. If you want to export your Keygpg to GitHub then: `gpg --armor --export <key>` and add this key to GitHub at GPG keys: https://github.com/settings/keys (with START and END line included)