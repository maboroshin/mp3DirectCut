# mp3DirectCut 日本語化ファイル

[mp3DirectCut](http://mpesch3.de/) の ver 2.25 の日本語化ファイルを作りました。開発者に連絡がとれたので、2019年11月のver2.26の本家のインストーラーに組み込まれています。

# DLLの入手先
[rarewares](http://rarewares.org/) から以下をダウンロードし、プログラムと同じフォルダに入れると機能が拡張されます。
* `lame_enc.dll` (32bit) 無劣化での編集ソフトだけど、mp3をエンコードもできるのでそうしたい場合。
* `libfaad2.dll` (32bit) AAC (`.aac`) を再生・編集する際に入れる。

[ffmpeg](https://www.ffmpeg.org/download.html) を使って、mp4 (`mp4`や`m4a`)も編集できるようです。その場合、入手した `ffmpeg.exe` を設定から指定します。プログラムと同じフォルダに入れた場合はファイル名を指定するだけです。（対応ファイルのより詳しい情報: [Yahoo!知恵袋](https://detail.chiebukuro.yahoo.co.jp/qa/question_detail/q11181589571)）

`mpglib.dll` は不要のようです。現在 より高速な ACM を使っており、 Windows 2000以前には mp3 の再生に `mpglib.dll` が必要だった様子。

# ポータブル化
インストーラーの拡張子を zip にして、[7-Zip](https://portableapps.com/apps/utilities/7-zip_portable)で解凍可能でした。「詳細設定」->「フォルダ」からポータブル化にチェックを入れると、設定をプログラムのフォルダに書き出します。