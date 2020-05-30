◎Flexboxとは◎
floatで作っていた横並びを、もっと簡単に作れるようになる便利なボックスです。
Flexboxを使うと、縦並び・横並び・ボックスの折返しを指定したりできます。

◎display: flexとは？◎
display: flexは指定した要素の子要素を横並びにします。
使い方は、横並びにしたい要素の親要素にdisplay: flexを指定します。

◎flex: autoとは◎
flex: autoは指定した要素の幅を親要素に合わせて伸縮させることができます。
使い方は、親要素の幅に合わせて伸ばしたい要素にflex: autoを指定します。

◎flex-wrap: wrap とは◎
flex-wrap: wrapを指定すると、子要素のサイズに応じて折り返すことができます。
使い方は、折り返したい要素の親要素にflex-wrap: wrapを指定します。折り返したい要素自身には列数に応じたwidthを指定します。
今回は2列にしたいのでwidth: 50%を指定しましょう。

◎flex-direction: columnとは◎
flex-direction: columnは子要素を上から下へ並べます。
使い方は、縦に並べたい要素の親要素にflex-direction: columnを指定します。
