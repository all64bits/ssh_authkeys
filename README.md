# Create authorized_keys file

Concatenate all contents of this repo & output to authorized_keys file

``` sh
$ find . -not -iwholename '*.git*' -type f -exec cat {} \; -exec echo -e '\n' \; > ~/.ssh/authorized_keys; chmod 600 ~/.ssh/authorized_keys
```
