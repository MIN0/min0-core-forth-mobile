MIN0 CORE FORTH Mobile Learning Web App

revision: ed91a2b

このZIPはWebサーバー配置用です。iPhoneの「ファイル」からindex.htmlを直接開いても
JavaScriptは実行されません。HTTPSの静的Webサーバーへ3ファイルを同じ場所に配置します。

- index.html
- manifest.webmanifest
- sw.js

iPhoneではSafariで配置先URLを開き、共有メニューの「ホーム画面に追加」で
「Webアプリとして開く」を有効にします。初回読込み後はservice workerが必要ファイルを
端末へ保存するため、オフラインでも起動できます。

このアプリは外部APIへFORTHソースを送信しません。保存先はブラウザのlocalStorageです。
