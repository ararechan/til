◎カプセル化
　「カプセル化」とは、オブジェクト指向の重要な機能の１つで、使い手に必要ないものを隠してしまうことを言います。
 　
  まずは、現実世界の例でカプセル化のイメージをつかみましょう。
　例えば、パソコンの回路はパソコンの内部に隠されており、ユーザーはキーボードなど限られた部分しか操作することができません。回路を隠す（カプセル化をする）と回路に触れてパソコンを壊してしまう危険を回避できます。
　プログラミングでもこのような「カプセル化」の仕組みがあります。
 
 ・クラスでのカプセル化
 　自分がクラスを作る際には他の人が安心してそのクラスを使えるように、他の人に使ってほしい機能は公開し、クラスの外で使ってほしくない機能は隠します。
　　使える機能を制限することで他の人はどの機能を使えばいいかが分かりやすく、また、安全にクラスを利用することができるようになります。
 
 ・フィールドとメソッドのアクセス制限
 　カプセル化とは、具体的にはフィールドとメソッドへのアクセスを制限することです。
   クラスの外部からアクセスできるようにするには「public」を、アクセスできないようにするには「private」を用いて定義します。
 
 ＜例、privateなインスタンスフィールドを定義する＞
    class Person {
      private データ型 インスタンスフィールド名
    }
    
◎ゲッター
　・クラス外からのアクセス
 　　フィールドのアクセス権をprivateにすると、フィールドにクラスの外からアクセスすることができなくなります。
　　 一方、privateでも、クラス内からはアクセスすることが可能です。
   
  ・ゲッター
  　フィールドをprivateにした上で、クラス外から安全にフィールドの値を取得するために、フィールドの値を返すだけのメソッドを定義します。これをゲッターと呼びます。
　　ゲッターは「getフィールド名」のように命名するのが一般的です。
    
    ＜例＞
      class Person {
        public 戻り値の型 getフィールド名() {
          // フィールドの値を返す
        }
      }
      
◎セッター
　・フィールドの値の変更
 　　フィールドのアクセス権をprivateにすると、当然フィールドの値をクラスの外から変更することもできなくなります。
   　
  ・セッター
  　そこで、フィールドの値を変更するメソッドを定義します。
　　このような、フィールドの値を変更するメソッドを特に「セッター」といいます。セッターは「setフィールド名」のように命名するのが一般的です。
  
  ・カプセル化の定石
  　何をprivateにし、何をpublicにするかというのは最初はよくわからないかもしれませんが、基本的なやり方があります。
　　最初のうちは、①フィールドはprivateに、②メソッドはpublicに、という2点沿っておけば、基本的に問題はありません。
  
   　＜例＞
      class Person {
        public void setフィールド名(データ型 仮引数) {
          // フィールドに値をセット
        }
      }
      
