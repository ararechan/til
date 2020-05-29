◎mainの構造◎
main要素は、「copy-container」、「contents」、「contact-form」の3つの要素で構成されています。

    <div class="copy-container"> --------------➜「copy-container」の<div>要素
    </div>

    <div class="contents">　　　　--------------➜「contents」の<div>要素
    </div>

    <div class="contact-form">　　--------------➜「contact-form」の<div>要素
    </div>

◎文中の一部にCSSを適用させる◎
文中の一部にCSSを適用させたい場合は、<span>要素で囲みます。<span>タグにCSSを指定することで、文字の色を一部変えています。
<span>要素の前後には改行は入りません。

◎ブロック要素・インライン要素◎
HTMLの要素には、改行される要素と改行されない要素があります。
前後で改行が入り、親要素の幅一杯に広がる要素をブロック要素といいます。
これまで勉強してきた<div>要素や<h1>要素、<p>要素はブロック要素です。それに対して、<span>要素や<a>要素のように改行されない要素をインライン要素といいます。

◎枠線をつけてみよう◎
要素にボーダー（枠線）をつけるには、borderプロパティを用います。図のように、枠線の太さ、種類、色を指定して使用します。
上下左右すべてに線を付けたい場合はborderとし、特定の場所にのみ付けたい場合は「border-bottom」のように、「border-方向」とします。
他にborder-top、border-left、border-rightなどがあります。

        【index.html】
        <div class="logo1">
          Progate
        </div>

        <div class="logo2">
          Progate
        </div>

        【stylesheet.css】
        .logo1 {
          border: 5px solid red;    -------------------➜太さ、線の種類、色
        }

        .logo2 {
          border-bottom: 1px solid #333;　　------------➜株に枠線がつく
        }

◎paddingとmargin◎
余白は、内側の余白と外側の余白の２つがあります。
内側の余白はpadding、外側に余白はmarginを用います。値の指定の方法は、paddingと同じです。

◎ボックスモデル◎
これまで勉強してきたborder, padding, marginは、ボックスモデルという概念に基いています。
HTMLの全ての要素には、border（初期状態では表示されない）があり、その外側の余白はmargin, 内側の余白はpaddingです。
marginもpaddingと同様に、各方向の余白をそれぞれ指定したり、まとめて指定したりすることも可能です。
