新潟市の割引の件で、PDFデータからcsvデータを生成するスクリプトです。

- 生成結果はdistに出力されています
    - csvには標準形式のcsvが出力されています
//     - jsonには https://niigata.stopcovid19.jp 用のjsonが出力されます
- 毎日定期的に自動で更新しています

## Requirement

- Python
- Pipenv
- Java 13

## Usage

```
# 割引券の使えるサイトに更新がある場合は手動で更新する
$ vim dist/csv/data.csv

# 市のページからCSVとJSONを生成する
$ pipenv run main

# 市のページからデータを取得する
$ pipenv run pdf

# 取得したデータから標準形式のCSVを生成する
$ pipenv run csv

# 標準形式のCSVからjsonを生成する
$ pipenv run json
```

## Install

```
$ pipenv install
```
