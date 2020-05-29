◎フッターのレイアウト◎
ヘッダーを作った時に<li>要素全体にfloatとpaddingを指定しました。これらは、フッターの<li>要素にも適用されてしまいます。
floatとpaddingをヘッダーの<li>要素にのみ適用されるようにするにはどうすればいいのでしょうか？

◎入れ子のセレクタ◎
下の図のように、「.header-list」の後にスペースを空けてliと続けると、「header-list」の中の<li>要素にのみCSSを適用することができます。
これにより、ヘッダーの<li>要素とフッターの<li>要素に別々のCSSを適用することができます。
 
   【index.html】
      <ul class="header-list">
        <li>ヘッダーのリスト</li>
        <li>ヘッダーのリスト</li>
      </ul>

      <ul class="footer-list">
        <li>フッターのリスト</li>
      </ul>

    【stylesheet.css】
      .header-list li {
        color: #ff0000;
      }
      
  ※こうすると「header-list」の子要素である<li>要素にのみCSSが適用される。
