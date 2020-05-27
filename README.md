# FRIDA-DEXDump

[Chinese WriteUp](https://mp.weixin.qq.com/s/x8_aa762wpsvA4nhSLoppQ)

Fast search and dump dex on memory.

## Features
1. support fuzzy search no-magic dex.
2. auto fill magic into dex-header.
3. compatible with all android version(frida supported).
4. support loading as objection plugin~

## Usage
1. update your frida-server and frida python binding to latest.
2. install require: `pip install -r requirements.txt`
3. launch app.
4. run: python main.py.
5. check `SavePath`.

### objection plugin

1. clone this repo to your plugins folder, eg:
    > git clone https://github.com/hluwa/FRIDA-DEXDump ~/.objection/plugins/dexdump
2. start objection with `-P` or `--plugin-folder` your plugins folder, eg:
    > objection -g com.app.name explore -P ~/.objection/plugins
3. run command:
    1. ` plugin dexdump search ` to search and print all dex
    2. ` plugin dexdump dump ` to dump all found dex.

## Screenshot

![](screenshot.png)
