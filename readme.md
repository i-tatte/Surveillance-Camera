# Surveillance Camera
## 何をするものなのか？

このプログラムは、外部のWebカメラから画像を取得し、何らかの動作を検知したときにアラートを鳴らすものである。
部室の窓枠にカメラを据え付け、先生の侵略からゲームをする部員を守ることを第一目的としている。
![sample.png](https://raw.githubusercontent.com/KEN-RP/Surveillance-Camera/master/sample.png)
![sample2.png](https://raw.githubusercontent.com/KEN-RP/Surveillance-Camera/master/sample2.png)
## 仕様

開発言語はJavaである。Webカメラの画像取得については、[sarxos氏](https://github.com/sarxos)の[webcam-capture](https://github.com/sarxos/webcam-capture)を使用した。ウィンドウ表示にはJavaFXを用いた。  
また、画像処理についてはImageUtilityクラスの中で逐一実装した。単に~~探すのめんど~~画像処理を実装してみたかっただけである。  
肝心の検知部分のアルゴリズムにはフレーム間差分法を採用した。  
現時点で最低限必要な機能はそろった。カメラの選択やGUIでの閾値の変更など、余力があれば機能を追加していこうと思う。
