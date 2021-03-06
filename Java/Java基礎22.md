【JAVAの演算子】

　◎算術演算子
 　算術演算子は、計算をするための演算子です。※インクリメントとデクリメントについては、変数の前につけるか後ろにつけるかで動作が少し異なる。


　＜例、算術演算子一覧＞
 
    演算子 　　	　名称	　　    　意味	　　　　　　　　　　　　　    例
      　
       +	  　　　足す	　　    値を加算する。（a＋b）	　　　　　　 2+3 → 5
    　　-	        引く	     　値を減算する。（a－b）	           2-3 → -1
       *	      掛ける	       値を掛ける。（a×b）	             2*3 → 6
       /	       割る	　　　　 値を割る。（a÷b）	               1/2 → 0.5
       %	       余り	        値を割った余りを求める。（…）	       3%2 → 1
       ^	      べき乗	       値を乗算する。（ab）	            2^3 → 8
      ++	    インクリメント	    値に１を加算する。（a＋1）	         2++ → 3
      --	     デクリメント	    値に１を減算する。（a－1）	         2-- → 1
    
    
  ◎代入演算子
　　代入演算子は、変数への値の代入を行う演算子です。「=」以外は代入と計算を同時に行います。
  
　　＜例、代入演算子一覧＞
      
    演算子 　　	　名称	　　    　意味	　　　　　　　　　　　　　    例
      =	　　　　　 代入	      値を代入する	i=2
      +=	　　　 加算代入	    a+=b は a=a+b と同じ意味	      2+=3 → 5
      -=　　　　　減算代入	    a-=b は a=a-b と同じ意味	       2-=3 → -1
      *=	      乗算代入	   a*=b は a=a*b と同じ意味	        2*=3 → 6
      /=	      除算代入	   a/=b は a=a/b と同じ意味	        1/=2 → 0.5
      %=	      余り代入	   a%=b は a=a%b と同じ意味	        3%=2 → 1
      
  
  ◎比較演算子
  　比較演算子は、２つの値を比較してboolean値で結果を戻す演算子のこと。
   
   ＜例、比較演算子一覧＞
   
     演算子 　　	　名称	　　    　意味	　　　　　　　　　　　　　    例
      <	　　　　　小なり	     左辺が右辺よりも小さい	             5<5 → false
    　<=	　　　小なりイコール	  左辺が右辺よりも小さいか等しい	       5<=5 → true
    　>	　　　　 大なり	     左辺が右辺よりも大きい	            5>5 → false
    　>=	     大なりイコール	  左辺が右辺よりも大きいか等しい	       5>=5 → true
    　==	        等しい	      左辺と右辺が等しい	                5==5 → true
    　!=	      等しくない	     左辺と右辺が異なる	               5!=5 → false
     
 ◎論理演算子
 　論理演算子は、１つ以上のboolean値を評価して結果をboolean値で戻す演算子のこと。
  
  ＜例、論理演算子一覧＞
  
     演算子 　　　	　名称	　　    　　　意味	　　　　　　　　　　　　　    
      &	　　　　　　論理積(AND)	　　左辺と右辺が両方ともtrueの場合にtrueを返す。
　　　　　　　　　　　　　　　　　　　　（左辺がfalseの場合でも右辺を評価する。）
　　　&&	　　　　　　論理積(AND)	　　左辺と右辺が両方ともtrueの場合にtrueを返す。
　　　　　　　　　　　　　　　　　　　　（左辺がfalseの場合は右辺は評価しない。）
　　　| 	          論理和(OR)	     左辺と右辺のどちらかがtrueの場合にtrueを返す。
                                 （左辺がtrueの場合でも右辺を評価する。）
    ||	          論理和(OR)	     左辺と右辺のどちらかがtrueの場合にtrueを返す。
                                 （左辺がtrueの場合は右辺は評価しない。）
     !            否定(NOT)	      trueの場合はfalse、falseの場合はtrueを返す.
     
