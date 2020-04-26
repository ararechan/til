・break
  繰り返し処理を終了するためには、条件をfalseにする以外に、breakを使って強制的に終了させる事ができる。
  if文などの条件分岐と組み合わせることで、任意の箇所で繰り返し処理を終了させることができる。

・continue
  breakと違い、continueはその周の処理だけをスキップして、次の周を実行することができる。
  continueもif文などと組み合わせて利用するのが一般的。

＜例、break＞

    int i = 1;
    for (int i = 1; i < 5; i++) {
      if (i == 3) {
        break; // ここでfor文が中断される
      }
      System.out.println(i);
    }

    // 出力: 1 2

＜例、continue＞

    int i = 1;
    for (int i = 1; i < 5; i++) {
      if (i == 3) {
        continue; // ここで処理がストップして、次のループを実行する
      }
      System.out.println(i);
    }

    // 出力: 1 2 4
