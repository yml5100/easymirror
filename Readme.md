# ■easymirror使用方法（テスト版）
![コメント 2024-11-21 095132](https://github.com/user-attachments/assets/89e474ae-d666-4b3a-b6c5-3864239c68cb)

## ■はじめに
　この度はテストへのご参加ありがとうございます。
このアプリはAndroidスマートフォンの画面をPCに
映すミラーリングアプリとなっています。
ボイスチャットなどでスマホゲームをしながら画面共有
を行ったり録画した画面を編集してみてください。

　また、一人で開発しているため
どんなバグが出るかが未知数です（やばそうなバグは潰しましたが）
もしアプリの挙動がおかしいと感じたら臆せずタスクマネージャー
から「easymirror」と「adb.exe」（無ければ大丈夫です）のアプリを
強制終了させてください。

　このアプリはスマートフォン側でUSBデバックを有効にする必要が
ありますのでご了承ください。
USBデバッグについては別記載の「USBデバック起動方法」をご確認ください。

スマホからの音声出力はAndroid11以上で対応しています。

　最後にアンケートのご記入をお願いします。
動作環境やどんなバグが出たかを確認するためのアンケートですので
ご協力お願いします。
※qrコードを配布しています



# ■起動方法
MirorrApp.exeを開くとスタート画面が開きます。

# ■機能説明
#  MainWindow
    1かんたんスタート
        MirorrAppが開始されコントローラーと
        スマホ画面が表示されます。

    2録画フォルダ
        録画やスクリーンショットをしたファイルを
        閲覧することができます。

    3カスタマイズ
        CustomSettingWindowに移動します。
        MirorrAppを起動する際に詳細な設定を行うことができます。      
# Controller
![コメント 2024-11-21 095602](https://github.com/user-attachments/assets/22fdb0ce-06b4-4652-8617-cf81f272f8d6)

    スマホ画面が表示された際にコントローラーを表示しカスタマイズを行える画面

    1全画面表示ボタン（アイコン）
        全画面表示が行える

    2録画ボタン
        画面の録画を行える
    
    3スクリーンショットボタン
        画面のスクリーンショットが行える

    4カスタマイズ
	MainWindowにあるボタンと同様コントローラーから
	CustomSettingWindowに遷移する。

    
    ※全画面ボタンと録画ボタンは既定の値を
    　返すようになっているためカスタマイズ機能で入れた値は反映されません。


# CustomSettingWindow
![コメント 2024-11-21 095615](https://github.com/user-attachments/assets/96691bf7-dd30-4971-b4eb-aa07440dc252)


    MirorrAppを起動する際に詳細な設定を行うことが
    できます。
    各種設定を行ってから「MirorrAppStart」を押すと
    設定が反映されスマホ画面が表示されます。

    1無線起動
        チェックを入れると無線での起動を行える
	初回起動はUSB接続が必要です。
        
    
    2各種入力箇所
        最大FPS,ビットレート,ビデオバッファ、最大サイズの
        変更を数値で行える。
    
    3録画機能
        チェックを入れることで録画を開始できる

    4コーデック選択
        映像・音声コーデックの変更ができる
        音声を出さないことも可能
    
    5画面サイズの変更
        画面サイズの変更が可能

    6無線接続切断
        無線接続からの切断をします
       ※無線接続をしている場合にボタンが押せるようにしています
         有線に戻したい場合に使用してください。

    ※0や何も記載がない場合はデフォルトの値を
    　返すようにしています

    最大FPS　      60fps
    ビットレート　  8M
    ビデオバッファ  0ms
    最大サイズ     1024px


## ■必要機能要件（スマートフォン）
CPU:　	1.8GHz以上
メモリ: 3GB以上

## ■使用ライブラリ・素材
app
- scrcpy  
https://github.com/Genymobile/scrcpy

## ■免責
作者は、このソフトによって生じた如何なる損害にも、  
修正や更新も、責任を負わないこととします。  
使用にあたっては、自己責任でお願いします。 

何かあれば[アンケートフォーム](https://forms.gle/xqppvi1PdnVyThGj7)か、githubの[issues](https://github.com/na-tu0227/easymirror/issues)までお願いします。


## ■著作権表示
Copyright (C) 2024 na_tu0227

自分が書いた部分のソースコードは、MIT Licenseとします。

## ■更新状況
<pre>
ver.0.5.1 
・[docs]Readme更新
・[feat]録画をしている時に録画アイコンを表示するように変更。
・[fix refactor] 無線機能のソースコードをリファクタリングの実施。WirelessProcからプロセスを呼び出していたのをMainProcで呼び出すように修正、nullチェックも無くなる。
</pre>












