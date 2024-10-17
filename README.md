# Morph Documentation

Morph の Documentation の Repository です。

[Mintlify](https://mintlify.com/docs/quickstart)というフレームワークを使用しています。

Anthropic, Perplexity, Resend, Cursor, Elevenlabs なども Minlify を使用しています。

[https://mintlify.com/customers](https://mintlify.com/customers)

## Development

以下の手順でセットアップしてください。

**1. Mintlify のインストール**

```
npm i -g mintlify
```

**2. ローカルサーバーの立ち上げ**

```
mintlify dev
```

## ディレクトリ構造

- `docs/`: ドキュメントの Markdown ファイル
- `asstes/`: 画像などの静的ファイル
- `examples/`: サンプルコード集ページ用のファイル

その他、独立したページ群を作る際にはルート直下にディレクトリを切ってください。

ここでいう「独立したページ群」は、Mintlify のタブで管理されるグループを指します。

## mint.json

各ページは MDX で記述することができますが、それを実際のページに反映するには、mint.json を編集する必要があります。

詳しい設定は Mintlify のドキュメントを参照してください。

よく使う項目については、以下で解説します。

### navigation

mint.json の navigation は、ページのグループを宣言するための項目で、navigation を設定することで、サイドバーやタブでそのグループを使用することができます。そのため、 **ページを追加したら必ず navigation にも設定を追加してください。**

```json
{
  "navigation": [
    {
      "group": "Get Started",
      "version": "en",
      "pages": [
        "docs/en/introduction",
        "docs/en/quickstart",
        "docs/en/development"
      ]
    }
  ]
}
```

# Contributing

main ブランチが自動的にデプロイされます。作業は、ローカルでブランチを作成して、main に向けて PR を作成してください。

PR マージ後はブランチを削除してください！

-
