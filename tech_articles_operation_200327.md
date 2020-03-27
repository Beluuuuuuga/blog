日本語名：技術記事の運用法

## はじめに
Qiitaが個人の読んだ記事の傾向を合意無しに表示し炎上しました。この件に関して、Qiitaをやめるべきかどうかまでは考えてはいませんが、今後Qiita自体の存在がなくなってしまう可能性もあるので、どのような運用で技術記事を活用するかを紹介します。

## 運用法
google docで技術記事を管理している方がおり、自分もこのような運用を考えました。google docのようなプレーンテキストではなく、Markdownでの運用がしたかったので、Githubでの技術記事運用を考えました。

## Githubでの運用法
Githubのコードを公開するためには、Gistsというサードパーティーの機能が存在しており、Gists内にファイルをコピーアンドペーストすることで外部にコードを表示できるようです。
しかし、リポジトリにコードが存在する場合、二重管理になってしまい好ましくありません。そこで、Githubのリポジトリのコードを張り付ける方法を探しました。
具体的な方法としては、以下のコードをブログに貼ることで、表示が可能です。

```
<script src="https://gist-it.appspot.com/github/Beluuuuuuga/blog/blob/master/tech_articles_operation_200327.md"></script>
```
gistライクなgist-itでは、以下のようにブログに貼ることでコードが公開可能だと言っていますが、はてなブログの場合httpsでないと表示されないので注意が必要です。

> <script src="http://gist-it.appspot.com/github/robertkrimen/gist-it-example/blob/master/example.js"></script>

また、ファイル名が**日本語**の場合もコードが表示されませんでした。英数字にしてください。

## 資料
#### Gistについて
- [はてなブログ　Gistでソースコード表示](http://gjjjjcdssvgg.hatenablog.com/entry/2018/08/04/224124)<br>
こちらははてなブログでのGistの使用法です。はてなブログでは、Gistのコードを張り付ける機能が存在してます。
- [GitHub Gistの使い方：コードをWordPressに埋め込み共有する方法](https://koskywalker.com/github-gist-use/)<br>
Gistについての説明です。

#### gist-itについて
- [gist-it.appspot.com](http://gist-it.appspot.com/)<br>
Gistライクに使用できるgist-itの英語記事です。自分のGithubのパスと見比べて使用してください。
- [gist-itを使って、はてなブログにGitHub上のコードをGist風に埋め込む方法](https://acokikoy.hatenablog.com/entry/2018/12/24/091946)<br>
git-itで具体的な使用法を紹介してます。一番参考になりました。
- [はてなブログにGithubコードを埋め込む](https://qiita.com/sikeda107/items/c35fb9327ab7f3f46cf5)<br>
上記で指摘したhttpsだと表示されない問題点を紹介しています。
