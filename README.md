# kuri-megane profile

くりメガネのプロフィールを管理するレポジトリです。

## 事前準備

- node, npm, yarn, nvmを必要とします
- nodeバージョンは、package.jsonに記載されています

```Shell
yarn install
```

## 使用しているライブラリ

- 文章構成 [textlint](https://github.com/textlint/textlint)
- プレコミットフック [husky](https://github.com/typicode/husky)
- マークダウンからPDF [md-to-pdf](https://github.com/simonhaenisch/md-to-pdf)

## 文書作成方法

適用されるtextlintのルールの詳細は [Github](https://github.com/textlint/textlint/wiki/Collection-of-textlint-rule) を参考にしてください。

### lintによる文章構成

```Shell
yarn lint
```

プルリクエスト作成時、masterマージ時にCIでも実行されます。

#### pdf生成

```Shell
yarn build:pdf
```
新しいリリースタグを作成したときにCIでも実行されます。

## デプロイ

Githubのリリース機能よりタグを打ってください。
cf. [リポジトリのリリースを管理する](https://docs.github.com/ja/repositories/releasing-projects-on-github/managing-releases-in-a-repository)
