このプログラムは、情報を書き込みたいGoogleSpreadSheetにユーザー名、内容をJavascript経由でGAS(Google Apps Script)に送信し、スプレッドシートに書き込むプログラムです。

※注意　
シートを作るときはGoogleアカウントが必要です。
シートの設定は、「リンクを知っている全員」で、閲覧者、閲覧者（コメント可）、編集者　のどれかでないといけません。限られた人の設定（学校、企業内）では使用することが出来ません。
スプレッドシートには、GASのプログラムが必要です。以下のプログラムをデータを入れたいプログラムのスプレッドシートのGASに入手してください。


function doPost(e) {
  var sheet = SpreadsheetApp.getActiveSpreadsheet().getActiveSheet();
  var username = e.parameter.username;  // ユーザー名を取得
  var inputData = e.parameter.inputData;  // 入力データを取得
  
  // ユーザー名と入力データを新しい行に追加
  sheet.appendRow([username, inputData]);
  
  // 成功メッセージを返す
  return ContentService.createTextOutput("Success");
}


<前提>
リンクを知っている全員（閲覧者、閲覧者（コメント可）、編集者　どれでも可）で共有されているGoogleスプレッドシート（GAS入手付み）


