◎HTMLの仕組み◎
HTMLでは、テキストに「タグ」と呼ばれる印を付けていきます。図のようにテキストをタグで囲むことにより、テキストが「見出し」や「リンク」といった意味をもつことになります。

◎開始タグと終了タグ◎
テキストをタグで囲む時は、以下の図のように、開始タグと終了タグではさみます。終了タグには「/」が必要な点に注意してください。

◎見出しをつける◎
見出しの要素は<h1>要素以外にも、<h2>, <h3>, ..., <h6>要素があります。hはheading（見出し）の略です。
図のように、<h1>が一番大きな見出しで、<h6>が一番小さな見出しになります。

◎段落を作成する◎
段落を表すのは<p>要素です。pはparagraph（段落）の略です。
<h2>要素や<p>要素で囲んだテキストは改行されます。

◎見出しと段落◎
<h1>, <h2>, ..., <h6>要素は、以下の図のように、見出しの大きさや重要性に応じて使い分けていきます。
見出し以外の文に関しては、<p>要素を用いましょう。

◎コメント◎
<!-- -->で囲んだテキストのことを「コメント」と呼びます。
コメントとして書かれたテキストはブラウザには表示されないので、メモとして使うことができます。
