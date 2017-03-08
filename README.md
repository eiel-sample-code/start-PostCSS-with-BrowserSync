# これは何?

PostCSS が試せるようにPostCSSとBrowserSyncでシンプルに構築してみたものです。

# 前提

* nodejs がインストールされている
* yarn がインストールされている

# 準備

```
$ yarn intsall
```

# 利用方法

```
$ yarn serve
```

`public`ディレクトリをドキュメントルートにBrowserSyncが起動します。
また、`src/css/**.css`を更新すると `public/css/`に変換後のファイルが生成されます。

現在はautoprefixerが設定していません。他のPostCSSのプラグインを利用したい場合は`package.json`の`scripts.watch:postcss`のpostcss-cliへの引数を調整してください。

* [postcss-cli 2.6.0](https://github.com/postcss/postcss-cli/tree/2.6.0)
