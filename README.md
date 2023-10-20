# git-scrypt

Dependencies: `bash`; `GPG`; `OpenSSL`; `git-crypt` and `base64`.

```
Usage: $(basename $0) COMMAND
Save a git-crypt key into your repository as an encrytped file.

  COMMAND
    e,encrypt    extact key and save it to '$asc'
    d,decrypt    decrypt key from '$asc' and set it locally
    i,init       initialise git-crypt: create a new key
```

It uses 500-1000 bytes of padding either side of the key. It works only for the (typical) "default" git-crypt key; if you have an unusual setup, this might not work.
