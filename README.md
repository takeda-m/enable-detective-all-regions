# Enable Amazon Detective in all regions

Amazon Detective を全リージョンで有効にするスクリプトです。

## 実行方法

このスクリプトは CloudShell にて実行することが可能です。

### 1. CloudShell を起動する

- AWS マネジメントコンソールの [>_] アイコンをクリックして CloudShell を起動する (画面右上のアカウント名の隣)

### 2. スクリプトをダウンロードする

- 「git clone」でスクリプトをダウンロードする。

```sh
$ git clone https://github.com/takeda-m/enable-detective-all-regions
```

### 3. スクリプトを実行する

1. 「cd」でディレクトリ enable-detective-all-regions へ移動する。
2. enable-detective-all-regions.sh を実行する。

```sh
$ cd enable-detective-all-regions/
$ ./enable-detective-all-regions.sh
```

### 4. ログを確認する

- エラーが発生していないか、ログを確認する。

```sh
$ grep ERROR enable-detective-all-regions.log
$ # ERRORメッセージがヒットしなければ正常です。
```
