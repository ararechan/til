◎真偽値を返す
　　・真偽値のデータ型はbooleanなので、メソッド定義は下図のようになります。
    isEvenメソッドは引数の値が偶数かどうかを調べ、偶数であればtrue、奇数であればfalseを返します。
    
    ＜例＞
    　public static boolean isEven(int a) {
       return a % 2 ==0;
      }
      　　　　　　⬇
            ２で割った余りが０（つまり偶数）であればtrue
            
     
◎クラスについて学ぶ
　
 ・複数のクラスを使う
 　クラスは、メソッドという小さな部品をまとめる、より大きな部品です。
   これまではmainメソッドと同じクラス（Mainクラス）のメソッドを使ってきましたが、他のクラスのメソッドを利用することも可能です。
   
 。クラスの定義
 　クラスの定義は「class クラス名」とします。
   また⬇の図のように、クラス名の最初の文字は大文字にし、ファイル名は「クラス名.java」としなければなりません。これらのルールはしっかり覚えておきましょう。 
   
   ＜例、クラスの定義＞
     class クラス名 {
       //ここにメソッドを定義
     }
     
    ＜例、命名規則＞ ※ファイル名とクラス名は大文字で書くこと！！
     class Person {
       //ここにメソッドを定義
     }
    　
  ・Personクラスを作ろう
  　　Personクラスを作り、Mainクラスのmainメソッド以外をPersonクラスに移します。
    　こうすることで、mainメソッド以外の「ロジック（論理）」部分をPersonクラスにまとめ、実行部分とロジック部分を切り分けることができます。
    　このように分割することで、Mainクラスは実行用のクラス、Personクラスはロジックをまとめるクラスという役割分担が明確になります。
     
  
  ・Personクラスのメソッドを呼び出す
    　Mainクラスのmainメソッドから、Personクラスのメソッドを呼び出してみましょう。
     
     ＜例＞                                                   
     【Main.java】                                           　
     class Main {                                            
       public static void main(String[] args) {
         String name = Person.fullName("Kate", "Jones");
         System.out.println(name);
       }
     }
    　
     【Person.java】
     class Person {
     
       public static String fullName(String firstName, String lastName) {
        return firstName + "" + lastName;
       }
       
     }
     
       ＜出力結果＞
       Kate　Jones
       ※PersonクラスのfullNameメソッドを呼び出ししている。
 
 
　・クラスの補足
 　　Javaは、ファイルではなくクラスを実行します。
   　また実行時にmainメソッドが呼ばれますが、正確にはmainメソッドを持つクラスしか実行できません（mainメソッドのないクラスは、他クラスから呼び出して使います）。
　　　またクラス名に関係なく、実行時にはmainメソッドが呼ばれます（Mainクラスだからmainメソッドが呼ばれる、というわけではありません）。
