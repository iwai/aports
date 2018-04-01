## Add repository

```conf:/etc/apk/repositories
http://dl-cdn.alpinelinux.org/alpine/v3.7/main
http://dl-cdn.alpinelinux.org/alpine/v3.7/community
https://iwai.github.io/aports
```

## Package install

```sh
# apk update --allow-untrusted
fetch http://dl-cdn.alpinelinux.org/alpine/v3.7/main/x86_64/APKINDEX.tar.gz
fetch http://dl-cdn.alpinelinux.org/alpine/v3.7/community/x86_64/APKINDEX.tar.gz
fetch https://iwai.github.io/aports/x86_64/APKINDEX.tar.gz
v3.7.0-140-g86561a5df4 [http://dl-cdn.alpinelinux.org/alpine/v3.7/main]
v3.7.0-139-g766e80ac96 [http://dl-cdn.alpinelinux.org/alpine/v3.7/community]
target  [https://iwai.github.io/aports]
OK: 9052 distinct packages available

# apk add --allow-untrusted tcp_wrappers
(1/1) Installing tcp_wrappers (7.6-r0)
Executing busybox-1.27.2-r7.trigger
OK: 4 MiB in 12 packages
```
