# [セキュアベースライン] Amazon Detective 全リージョン有効化スクリプト

Amazon Detective を全リージョンで有効にするスクリプトです。

## 実行方法

このスクリプトは CloudShell にて実行することが可能です。

### 1. CloudShell 起動

- AWS マネジメントコンソールの [>_] アイコン(画面右上のアカウント名の隣)をクリックして CloudShell を起動します。

### 2. スクリプトダウンロード

- 「git clone」でスクリプトをダウンロードします。

```sh
$ git clone https://github.com/takeda-m/enable-detective-all-regions
```

### 3. スクリプト実行

1. 「cd」でディレクトリ enable-detective-all-regions へ移動します。
2. enable-detective-all-regions.sh を実行します。

```sh
$ cd enable-detective-all-regions/
$ ./enable-detective-all-regions.sh
# 以下のINFOメッセージが表示されれば実行終了です。
2022-09-20T03:08:27 [INFO] (enable-detective-all-regions.sh:111:main) 全リージョンのAmazon Detectiveを有効化 正常終了
```

### 4. ログ確認

- エラーが発生していないか、ログを確認します。

```sh
$ grep ERROR enable-detective-all-regions.log
$ # ERRORメッセージがヒットしなければ正常です。
```
