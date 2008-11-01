Title      : DocLink
Category   : Snippet
Author     : Phize
Author URI : http://phize.net
License    : GNU General Public License(http://www.gnu.org/licenses/gpl.html)
Version    : 1.0.0
Last Update: 2008-11-01



0.目次
------

1.概要
2.インストール
3.使い方
4.パラメーター



1.概要
------

DocLinkは、前後のドキュメントへのリンクを表示するスニペットです。
前後へのリンクのほかに、最初のドキュメント、最後のドキュメント、ホームページへのリンクも表示できます。

出力するXHTMLはテンプレートファイルで完全にカスタマイズが可能です。
あらかじめ同梱されているテンプレートとCSSを利用することで、
簡単に見栄えのするナビゲーションを作成することもできます。

また、link要素を出力するテンプレートを利用することによって、
検索エンジンなどに対しても優しいサイトになります。



2.インストール
--------------

1.doclink/フォルダを /assets/snippets/ にコピー。

2.「DocLink」という名前のスニペットを新規作成。

3.doclink.snippet.tpl.phpの内容を「スニペットコード」にコピー&ペースト。

4.スニペットを保存。



3.使い方
--------

標準では、前後のドキュメントへのシンプルなナビゲーションリンクを表示します。
表示したいドキュメントの中でスニペットをコールします。

  [[DocLink]]


link要素を出力する場合:


ナビゲーション用のlink要素を出力する場合:
  <head>
    ...省略...
    [[DocLink? &template=`link` &style=`none`]]
  </head>



4.パラメーター
--------------

パラメーターを指定することで、見栄えや機能を変えることができます。
詳しくは、同梱のDocLink.ja.pdfを参照してください。
