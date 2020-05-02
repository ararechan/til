◎ライブラリ
　・外部ライブラリとは？
 　　Javaでは、他人が作ったクラスを利用することもできます。
   　このようなクラスを外部ライブラリと呼び、自分のプログラムに読み込むことで利用できるようになります。
    すべてのプログラムを自分だけで開発する必要はありません。世界中のエンジニアが作った便利なメソッドを利用することで、開発の幅は一気に広がります。
    
  ・外部ライブラリのimport
  　外部ライブラリを自分のプログラムに読み込む（使えるようにする）には、importを用います。
　　数学的なメソッドを持つMathというクラス（ライブラリ）を読み込むには、class定義より上で「import java.lang.Math」とします。
　　「java.lang」の部分は、Mathクラスの場所を示しているという程度に覚えておきましょう。
  
  ＜例＞
    import java.lang.Math; ※外部ライブラリを読み込む
    
    class Main {
      public static void main(String[] args) {
        :
        :
        :
      }
    
    }
 
 ・maxメソッド
 　maxメソッドは、引数に渡した2つの数値の大きい方を返してくれます。外部ライブラリをうまく活用すれば、自分で実装する手間が省けるので便利です。
  
 ・roundメソッド
 　引数の小数点以下を四捨五入して返すメソッドのこと。これはdouble型の引数を渡し、Math.round(引数)のように使います
  
◎入力を受け取る
　
 ・import不要のクラス
 　先ほど読み込んだ「java.lang.Math」はよく利用されるため、実は特別にimportせずに自動で読み込まれるようになっています。
   Mathクラス以外にも「java.lang.クラス名」となる外部ライブラリはすべて自動で読み込まれます。
   
 ・コンソールへの入力とScanner
 　これまではコンソールに値を「出力」してきましたが、実は左の図のようにコンソールに値を「入力」し、その値をプログラム内で使うこともできます。
　 コンソールへの入力を受け取るにはScannerというライブラリを用います。Scannerは「import java.util.Scanner」と読み込みます。
 　ライブラリは、Googleで検索すれば使い方がわかりますので、覚える必要はありません。
  
 ・Scannerで文字列を受け取る 
 　Scannerの使い方を見てみましょう。
 　まずScannerを初期化しscannerという変数にいれています。
 　詳しくはまだ知らなくて大丈夫ですが、Scannerではこの初期化したものを代入した変数を使ってメソッドを呼び出します。
 　scanner.next()とすると（Scanner.next()とは違う）、コンソールに入力された文字列を受け取ることができます。
  
 ・Scannerの処理の流れ
 　Scannerの処理の流れを確認しましょう。
 　scanner.next()が呼ばれると、一旦処理が中断しコンソールに値が入力されるのを待ちます。
 　左の図では、コンソールに入力された値をscanner.next()が受け取り、変数nameに代入しています。
  
  ＜Scannerの使い方の例＞
  
      import java.util.Scanner;
      class Main {
        public static void main (String[] args) {
          Scanner scanner = new Scanner(System.in);

          // コンソールから文字列を受け取り、変数textに代入する
          String text = scanner.next();

        }
      }
      
   ・数値の入力を受け取る
   　Scannerを用いて整数を受け取るメソッドはnextIntメソッド、小数を受け取るメソッドはnextDoubleメソッドです。
    
    
