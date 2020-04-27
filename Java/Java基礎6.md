・拡張for文
  Javaには、配列とfor文を簡単に組み合わせるために、拡張for文が用意されています。
  普通のfor文ではインデックス番号を用いて配列の要素を取得しなければなりませんが、拡張for文では変数に配列の要素自体が代入されます。
  拡張for文の方がシンプルに書けることが多いので覚えておきましょう。

　　＜例＞
      String[] names = {"Bob", "Kate"};
      for (String name : names) {
        System.out.println(name);
      }

      // 出力: Bob Kate
