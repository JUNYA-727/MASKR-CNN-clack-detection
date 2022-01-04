# Description
富士フィルムが開発している｢ひびみっけ｣と同様のプログラムをデータ収集からアノテーション､モデル作成､予測まで自身で作成した｡ひびみっけのモデルはどのように作成しているかは公開していないが､自身はMask R-CNNを用いて検出を行うモデルを作成した.
主にひびみっけはコンクリートのひび割れを検出して､検知を行い､未然に事故を防ぐ事に活用されている｡

(引用：https://www.fujifilm.com/jp/ja/business/inspection/infraservice/hibimikke
# Model Features
アノテーションを行ったjsonファイルからマスク画像を作成､Mask R-CNNを介して学習を行う｡
## 本来の画像とマスク画像
![11](https://user-images.githubusercontent.com/61785070/147964197-8647c376-b8c6-4a6a-b686-77b327744ef7.jpg)

## 予測結果
![ダウンロード (4)](https://user-images.githubusercontent.com/61785070/147964252-9888d331-5def-4a63-aa1a-645769a1dd46.png)
![ダウンロード (5)](https://user-images.githubusercontent.com/61785070/147964273-d472aeac-e510-4b2c-b584-13ebea38e4fd.png)
![ダウンロード (6)](https://user-images.githubusercontent.com/61785070/147964284-87f42a25-f5af-4bbc-8ed6-9bfccf9ae000.png)

## 考察
Mask R-CNNは様々な現場で活用が可能である｡今回は建設現場での利用状況が多いコンクリート画像で学習を行ったが､学習するデータを医療用画像やX線画像等で用いる事で症状の発見を手助けする事ができると予想できる｡

(引用：https://www.jstage.jst.go.jp/article/mit/38/3/38_126/_pdf)
