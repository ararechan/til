◎HTMLの構造◎
実際のHTMLファイルには、決められた型を書いていく必要があります。
図のように、<html>要素の中に<head>要素と<body>要素が必要です。<head>要素にはページに関する情報、<body>要素には実際に表示したい内容を書きます。
これまで勉強してきた要素は、<body>要素の中に記述していきます。

◎HTMLバージョンを指定する◎
<!DOCTYPE html>の部分はDOCTYPE宣言と呼ばれるもので、HTMLのバージョンを宣言するためのものです。
今回は最新バージョンのHTML5を使うため、<!DOCTYPE html>を使用します。
この辺りは特に気にせず、必ず記述するものだと覚えておきましょう。

◎<head>要素について◎
<head>要素にはWebページの設定に関する情報を書いていきます。<head>要素内に記述した内容はWebページには表示されません。

◎<head>要素の中身◎
<head>要素の中では、以下のように①文字コードの指定、②ページのタイトルの設定、③CSSの読み込みなどを行っていきます。
これらは定型文のようなものなので完全に覚える必要はありませんが、どのようなものがあるのかを知っておきましょう。

    <head>
      <meta charset="utf-8">
         ➜文字コード
      <title>Progate</title>
        ➜ページタイトル
      <link rel="stylesheet" href="stylesheet.css">
        ➜CSSの読み込み
    </haad>

◎<head>の中身①文字コードを指定する◎
文字コードを指定することで、ページの文字化けを防ぐことができます。<meta charset="utf-8">とすることで、そのページの文字コードをUTF-8に指定することができます。
UTF-8は、HTML5で推奨されている文字コードです。

◎<head>の中身②ページのタイトルをつける◎
<title>要素は、ページのタイトルを指定します。<title>要素で指定されたタイトルは、ブラウザのタブ上に現れます。

◎<head>の中身③CSSの読み込み◎
これまでProgate上では「stylesheet.css」で記述したCSSが結果に反映されていましたが、本来はHTMLの方で読み込む必要があります。
HTMLからCSSを読み込むためには、<link rel="stylesheet">を用います。
<link rel="stylesheet" href="stylesheet.css">のように、href属性で読み込むCSSファイルを指定します。

 rel="stylesheet"がCSSを読み込む宣言。
 
 href="stylesheet.css"が読み込むCSSのファイル。
 
