◎クラスの定義◎
    
    class クラス名 {
      // インスタンスフィールドの定義
      private データ型 フィールド名;
      
      // インスタンスフィールドに初期値を設定する
  　　 private データ型 フィールド名 = 初期値;

      // コンストラクタの定義
      クラス名(データ型 仮引数, ・・・) {
        // 処理
      }
      
      // インスタンスメソッドの定義
      public 戻り値の型 メソッド名() {
        // 処理
      }
      // runメソッドのヒント
      public 戻り値の型 run(データ型 仮引数) {
        // 処理
      }
    }
ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー

◎ Main.Java
   
  　 // Scannerの使い方(ライブラリをimport)
   import java.util.Scanner;
   
   class Main {
      public static void main (String[] args) {
      
          // Scannerを初期化
        Scanner scanner = new Scanner(System.in);
      
        　// インスタンスの生成と変数への代入
        クラス型 変数名 = new クラス名(引数, ・・・);
        
        　// 入力値の受け取り(文字列)
        String s = scanner.next();
        　// 入力値の受け取り（整数）
        int i = scanner.nextInt();
        　// 入力値の受け取り（少数点）
        double d = scanner.nextDouble();
        
      }
    }
ーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーーー

◎改行をしないで文字列を表示
   
   System.out.print("文字列");
