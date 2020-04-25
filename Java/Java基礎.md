＃progateでJava学習

＃＃Javaでアプリを作るため、基礎から勉強していきます。

◎条件分岐
　・プログラミングでは「特定の状況のときだけある処理を行う」をよく使う。このようなプログラムを条件分岐という。
　プログラミングで必須知識！！・条件分岐でよく使うのがif文。ifは英語で「もし〜なら」という意味。

　　if（条件式）｛
 　　処理；
 　　｝　

　　↑「〜」に当たる部分が、ifの後の（）の部分である。括弧の中は条件式と呼ぶ。ブラケットの中がtrueなら、｛｝中括弧の中に書いてある処理が行われる。

　・if文は｛｝を使う。
　　複数の処理をまとめたいときに使う。ブロックという。{ }の後ろにはセミコロンは不要。

　・elseを使った条件分岐
　　elseとは英語で「そのほかの」というような意味。ifとelseを組み合わせて「もし〜なら◯◯、そうでなければ△△」という条件分岐が可能となる。
　　※｛｝の使い方、位置を覚えるようにする。
 
  　　＜elseの使い方① trueの場合＞　結果：xは３０より小さい
  　　　int x = 20;
  　　　if (x < 30){
    　　　System.out.println("xは３０より小さい");  
  　　　} else {
    　　　System.out.println("xは３０以上");
  　　　}
  
  　　＜elseの使い方②　falseの場合＞　結果：ｘは３０以上
  　　　int x = 40;
  　　　if (x < 30){
    　　　System.out.println("xは３０より小さい");  
  　　　} else {
    　　　System.out.println("xは３０以上");
  　　　}
  
 　・else if
  　条件分岐のの中に更に条件分岐を入れることができる。
   「if」と「else if」と「else」を組み合わせると、「もし〜なら◯◯、そうではなくてもし××なら△△、どちらでもない場合は□□」が出来る。
  
  　　＜例①falseとtrueの場合＞　結果：xは２０より大きく、３０より小さい
       int x = 25;
       if (x >= 30){
         System.out.println("xは３０以上"); 
       } else if (x > 20){
         System.out.println("xは２０より大きく、３０より小さい");
       } else {
         System.out.println("xは20以下");
       }
       
      ＜例②falseとfalseの場合＞　結果：xは20以下
       int x = 15;
       if (x >= 30){
         System.out.println("xは３０以上"); 
       } else if (x > 20){
         System.out.println("xは２０より大きく、３０より小さい");
       } else {
         System.out.println("xは20以下");
       }
