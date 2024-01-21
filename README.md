# PR_Garbage-Detection（垃圾辨識系統）

## 問題描述
在當今社會中，垃圾管理和環境保護變得越來越重要。期望設計一個基於深度學習技術的垃圾辨識系統，旨在提高垃圾分類的效率，促進資源回收，以實現更可持續的環境發展。

## 方法
- 影像處理
- TensorFlow Protobuf
- 讀取圖像文件
- 回收分類

## 資料集
TACO 🌮 關於野生垃圾的open image dataset，環境從海灘到街景
- Official: 1500 images
- Unofficial: 3746 images
- Labels: 60 categories

## 訓練模型
- UFF file (.uff)
- TensorFlow frozen graph (.pb)
- TensorRT engine (.engine)
- SSD MobileNet v2
- TensorRT 6
- trained with 100,000 steps

## 不可回收項目 (一般垃圾) 和 可回收項目 (資源回收) 的列表

## 實驗
- 辨別垃圾 (簡單分類）
- Kaggle taco-trash-dataset
- Our Images: photos from google

## 限制
- Category Duplication
- Yellow will be recognized as Crisp packet
- Can’t work on GPU

## 預期成果
自動垃圾辨識模型 （期望：智能垃圾分類桶）
- 模型應用於垃圾分類桶
- 方便市民進行回收分類
- 有效提高垃圾處理效率

## 參考資料
- Taco Dataset http://tacodataset.org/
- Cleanrobotics https://cleanrobotics.com/
- Kaggle: TACO (Trash Annotations in Context) Trained Models https://www.kaggle.com/datasets/bouweceunen/trained-models-taco-trash-annotations-in-context/data
- TrashBot 推 18 萬元 AI 垃圾桶，讓消費者「無腦」丟垃圾 https://technews.tw/2022/09/11/clean-robotics-trashbot/

## Reference
- Training Data: [taco](http://tacodataset.org/) 
- Model: https://www.kaggle.com/datasets/bouweceunen/trained-models-taco-trash-annotations-in-context/data
