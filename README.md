# emotion_analyze
下記のコマンドでprep.shに実行権限を与える
```bash
chmod a+x prep.sh
```
```bash
./prep.sh
```
上記のコマンドでprep.shを起動すると、自動で必要なフォルダが作成され、必要なパッケージがインストールされる
preparation doneどでたら終了

##　動画を分析する方法
```python
python video.py [動画のパス]
```
保存先はvideo/folder*の中になり、新しく分析を実行する度に*の数字が更新される

##　ウェブカメラからの入力でリアルタイムで分析する方法
```python
python webcam.py
```
保存先はwebcam/folder*の中になり、新しく分析を実行する度に*の数字が更新される

##　分析後の出力

imagesには分析時にばらした連番の画像が入っている
log.csvには感情の割合、タイムスタンプ、分析した画像へのパスが記録される
result.mp4は分析し終わった画像を動画に変換した最終出力となっている
