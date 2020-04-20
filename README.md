# electron-minidump

Symbolicates Electron Windows crashes in minidump format. c.f. [electron-atos](https://github.com/nornagon/electron-atos).

To install: `npm install -g electron-minidump`.

```sh
$ electron-minidump --help
electron-minidump [args]

Options:
  --file, -f     path to minidump (.dmp) file                         [required]
  --version, -v  electron version                                     [required]
  --platform, -p platform, darwin/win32                               [required]
  
  --quiet, -q    suppress download progress output
  --force        redownload symbols if present in cache
  --help         Show help                                             [boolean]
```

```sh


$ electron-minidump -p darwin -f crash.dmp -v 3.1.0-beta.5

