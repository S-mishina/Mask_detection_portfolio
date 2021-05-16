## システムの内容
yolov5を利用したマスク検知プログラム<br>
具体的には,yolov5を利用し,マスクを検知<br>
その後,音声で結果を出力し,データベースに書き込み,webで可視化を行う.
## 実行方法
クライアント側<br>
$python detect.py --source 0の実行<br>
サーバ側<br>
$python server.py
## システムの構成
### 認識部分
detect.py内socket部分のipアドレス変更
### 音声出力部分
認識部分socketクライアントとパッケージAre-you-wearing-a-maskAPIとの連動<br>
データベースのipと設定を変更
### 可視化部分
パッケージAre-you-wearing-a-maskAPIとyolov5web-visualization-platformの連動<br>


