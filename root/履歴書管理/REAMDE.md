# はじめに

転職活動をしており、履歴書を作成する機会が多いです。ただ、履歴書の作成って面倒ではないですか？社用 PC ではないので、office 系のアプリケーションは使えないですし。。。
そこで、yaml 形式で内容を記載すれば、自動で履歴書を生成してくれる方法を探しましたので、備忘録がてら紹介します。

# 実行手順

履歴書を作成したいディレクトリを作成します。
今回は、/users/username/job というディレクトリを作成します。

```
mkdir ~/job
```

次に、[yaml_cv](https://github.com/ikasam/yaml_cv)というリポジトリをクローンします。

```
cd ~/job
git clone https://github.com/ikasam/yaml_cv.git
cd yaml_cv
```

必要モジュールのインストールを行います。

```
bundle config path vendor/bundle
bundle config set --local without 'documentation'
bundle install
```

以下コマンドで履歴書を作成します。

```
ruby make_cv.rb -i data.yaml -s style.txt -o output.pdf
```

このコマンドで、data.yaml というファリを style.txt に倣い、output.pdf という形式で出力します。

以上。

# 参考

[YAML で履歴書を作る](https://qiita.com/kaityo256/items/e3884d0109223c324baf)
