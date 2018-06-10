# techocean-application


リリース手順書
----------
1. リリース用ディレクトリを用意する

```bash
    $ cd /home/ipac/www/techocean.co.jp
    $ mkdir techocean-{v.v.v}-{YYYYMMDD}T{HHMM}
```

2. ファイルをアップロード

    WinSCPなどを経由で`./webapp/*` にあるファイルを`techocean-{v.v.v}-{YYYYMMDD}T{HHMM}` にアップグレードする


3. リリースする

```bash
    $ cd /home/ipac/www/techocean.co.jp
    $ ln -snf techocean-{v.v.v}-{YYYYMMDD}T{HHMM} lastest
```

4. 画面を確認する

    Browserなどを経由で https://techocean.co.jp/ をアクセスして、表示されている画面を確認する
