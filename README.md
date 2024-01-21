# PR_Garbage-Detection（垃圾辨識系統）

### 問題描述
在當今社會中，垃圾管理和環境保護變得越來越重要。期望設計一個基於深度學習技術的垃圾辨識系統，旨在提高垃圾分類的效率，促進資源回收，以實現更可持續的環境發展。

### Methods
- 影像處理
- TensorFlow Protobuf
- 讀取圖像文件
- 回收分類

### Dataset
TACO 🌮 關於野生垃圾的open image dataset，環境從海灘到街景
- Official: 1500 images
- Unofficial: 3746 images
- Labels: 60 categories

### Training Model
- UFF file (.uff)
- TensorFlow frozen graph (.pb)
- TensorRT engine (.engine)
- SSD MobileNet v2
- TensorRT 6
- trained with 100,000 steps

### Experiments
- 辨別垃圾 (簡單分類是否為回收物）
- Kaggle taco-trash-dataset
- Our Images: photos from google

**圖一：多個塑膠垃圾**
<img width="709" alt="Xnip2024-01-21_17-59-48" src="https://github.com/weipo0116/PR_Garbage-Detection/assets/80244742/67d75f74-810c-4a31-a1d7-43df84014162">

**圖二：麥香奶茶包裝**
<img width="416" alt="Xnip2024-01-21_17-59-58" src="https://github.com/weipo0116/PR_Garbage-Detection/assets/80244742/df3fc793-c695-42ee-914f-87d3261ee729">

### Limitation
- Category Duplication（如圖二）
- Lack of training data (Yellow will MOSTLY be recognized as Crisp packet)

### Reference
- Training Data: [TACO Dataset](http://tacodataset.org/) 
- Model: [TACO (Trash Annotations in Context) Trained Models](https://www.kaggle.com/datasets/bouweceunen/trained-models-taco-trash-annotations-in-context/data)
- idea:
  - [Cleanrobotics](https://cleanrobotics.com/)
  - [TrashBot](https://technews.tw/2022/09/11/clean-robotics-trashbot/)
