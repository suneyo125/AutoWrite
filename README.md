このプログラムは、情報を書き込みたいGoogleSpreadSheetにユーザー名、内容をJavascript経由でGAS(Google Apps Script)に送信し、<br>スプレッドシートに書き込むプログラムです。

<br>alert と textboxの違い
<br>url, ユーザ名, 内容をJavascriptのalertで聞くのがveralert, textboxで入力するのがvertextbox です。
<br>
<br>※注意　
シートを作るときはGoogleアカウントが必要です。
<br>シートの設定は、「リンクを知っている全員」で、閲覧者、閲覧者（コメント可）、編集者　のどれかでないといけません。限られた人の設定（学校、企業内）では使用することが出来ません。
<br>スプレッドシートには、GASのプログラムが必要です。以下のプログラムをデータを入れたいプログラムのスプレッドシートのGASに入手してください。

[GASprogram.txt](https://github.com/suneyo125/AutoWriteGoogleSpreadSheet/blob/main/GASprogram.txt)
<br>
<br>
<前提>
<br>1.リンクを知っている全員（閲覧者、閲覧者（コメント可）、編集者　どれでも可）で共有されているGoogleスプレッドシート（GAS入力付み）
<br>2.1のスプレッドシートをウェブアプリとし、自分として実行、全員アクセス可能にデプロイしたGAS
<br>
<br>
<br><使い方>
<br>1.送信ボタンを押す
<br>2.デプロイしたGASのウェブアプリのURLを入力
<br>3.ユーザー名を入力
<br>4.送りたい内容を入力
<br>"データの送信に成功しました"と入力されたら、完了です。お疲れ様でした！
