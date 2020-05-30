◎レスポンシブデザインとは◎
レスポンシブデザインとは、様々なデバイスや画面サイズに合わせて、コンテンツのレイアウトを調整するためのものです。
特にスマートフォン表示に対応したサイト制作においては必須の技術です。

◎メディアクエリ（Media Queries）とは◎
メディアクエリとは、ブラウザの画面サイズに応じてCSSのスタイルを設定できる手法です。
メディアクエリの書き方は、@media (条件) { .... }という様に書きます。指定された条件が当てはまるときにのみ{ }内のCSSが適用されます。

◎max-widthとmin-width◎
メディアクエリの条件には、max-width(最大幅)、またはmin-width(最小幅)を指定できます。
max-width: ◯◯pxと指定すると、画面幅が◯◯px以下の時にCSSを適用できます。min-widthはその反対となります。

◎ブレイクポイント◎
max-width: ◯◯px（またはmin-width: ◯◯px）のようにメディアクエリの条件を指定するとき、「◯◯px」の部分をブレイクポイントと呼びます。
今回はスマートフォンの画面幅は670px以下、タブレットの画面幅は670px ~ 1000pxと想定して、ブレイクポイントを設定しましょう。

◎レイアウト崩れを直す◎
widthを%で指定している際、左右のpaddingを追加するとレイアウト崩れが起きる場合がある。要素の幅の合計が100%を超えてしまうと、レイアウトが崩れてしまう。
このようなレイアウト崩れは、box-sizing: border-box;を用いることで防ぐことができます。

◎box-sizing: border-box;の仕組み◎
box-sizingをborder-boxに指定すると、要素の幅(width)の合計にpaddingとborderが含まれるようになります。
そのため、paddingやborderを追加した時に生じるレイアウト崩れを未然に防ぐことができます（※ただし、marginはborder-boxでの合計値に含まれません）。

◎全要素にCSSを適用する◎
box-sizing: border-box;を指定するときは、*(アスタリスク)に対して指定することが推奨されています。
*はすべての要素に対してCSSを適用したい場合に用います。
border-boxをすべての要素に対して適用することで、レイアウトを管理しやすくなります。
     
     ＜例＞
      /*HTML全体にbox-sizing: border-box;を適用*/
       ＊ {
         box-sizing: border-box;
       }

◎viewportの設定◎
レスポンシブデザインを適用する準備として、<head>タグ内にviewportを設定しましょう。
viewportを設定しないと、スマートフォンやタブレットでの閲覧時にメディアクエリが正しく機能しません。
ただし、ここでviewportの中身の書き方を暗記する必要はありません。

◎width: 100%◎
「ｐｘ」だとスマートフォンなどの小さい画面で見切れてしまいコンテンツが収まらなくなる。画面幅によって全体のwidthが変わるように、width: 100%;に変更しましょう。

◎floatと親要素の高さ◎
通常、親要素の高さは子要素を包む高さとなります。
しかし、子要素が全てfloatの時、親要素の高さは0となってしまうという性質があります。
これは、floatは「浮いている」という意味で、親要素から見るとfloatの子要素は存在しないように見えるからです。

◎floatの解除◎
floatはclear: left;で「浮いている」状態を解除できます。子要素が全てfloatでも、親要素が高さを持つように設定してみましょう。
HTMLファイルでclear: left;を適用するためだけの空のタグを用意しましょう。
空タグとclearでfloatを解除するのはよく使うテクニックなので、覚えておくようにしましょう。

◎フォントのレスポンシブ化◎
画面幅が小さいときは、フォントサイズを小さくしたほうが読みやすくなります。
画面幅によって、フォントサイズを調整していきましょう。

◎画面サイズが大きい時に対応しよう◎
ここまで、タブレットやスマートフォンなどの小さい画面でも綺麗なレイアウトで表示できるようにしてきました。
しかし、とても大きい画面ではどうでしょうか？
例えば2000pxの画面幅で表示すると、レッスン部分がお互いに離れすぎていて、見づらくなっています。これを直しましょう。

◎max-widthを指定する
ある要素のwidthが100%にした場合、画面幅が2000pxだと、とても大きい時も画面いっぱいに広がってしまいます。
max-width: ◯◯px;と指定すると、画面幅を拡大しても、要素の幅の上限が◯◯pxとなります。
　
     ＜例,書き方＞
       .container {
         max-width: 1170px;
         width: 100%;
       }

    ※画面幅の上限を指定して、その上限内で幅を最大まで広げる。
    
◎スマートフォンのヘッダーレイアウト◎
スマートフォンでのヘッダーのレイアウトを整えていきましょう。
スマートフォンでは、ヘッダーメニューを表示しきれないため、メニューをアイコンに変更します。
（本来はjQueryなどを用いてアイコンをクリックした時の動作をつけるべきですが、このレッスンでは扱いません）。

◎要素の表示/非表示◎
メニューアイコンはデフォルトでは非表示にし、画面幅が670px以下（スマートフォンサイズ）の時にのみ表示されるようにします。
要素を非表示にするにはdisplay: none;を用います。非表示にした要素を表示させる時は、display: block;を用いて表示します。
