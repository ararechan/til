◎余白の調整◎
要素に余白を作りたい場合は、paddingを用います。
「padding: 値;」とすると、上下左右すべての方向にその大きさの余白が追加されます。

◎paddingをある方向のみ指定する◎
上下左右ではなく、ある方向のみに余白を指定したい場合もあります。
その場合は、以下のように、「padding-top: 値;」などとすると、その方向のみに余白が追加されます。
他にpadding-bottom、padding-left、padding-rightなどがあります。

◎paddingをまとめて書く◎
指定したい値が方向ごとに異なる場合、個別で指定する方法もありますが、まとめて書くことも可能です。
値を4つ、スペース区切りで指定した場合、「上」「右」「下」「左」の順で適用されます。（上から時計回り）
値を2つ指定した場合、「上下」「左右」の順に適用されます。

    ＜paddingの書き方ー個別指定＞
     logo1 {
       padding-top: 20px;
       padding-right 10px;
       padding-bottom: 20px;
       padding-left: 10px;
     }

     ＜paddingの書き方ー省略①＞
     logo1 {
       padding-top: 20px 10px 20px 10px;
     }

      ＜paddingの書き方ー省略②＞
     logo1 {
       padding-top: 20px 10px;
     }
     
 　※上記３点の書き方はどれも同じ内容です。
 
 
