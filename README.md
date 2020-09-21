# well_known_id_rsa
A well known SSH key usable for automatic deployment *in a secure environment* (similar to a default password).

The idea is that you can build disk images with this SSH key as `authorized_key` so that you have a default login option. Then you can automatically deploy the system e.g. using ansible and replace the `authorized_key`s with your real SSH keys.

__⚠️ A word of warning: ⚠️__ Obviously this has the same implications like using a well-known password; e.g. a `root:root` login, so only use this in a secure environment and remove the key during setup/deployment!
