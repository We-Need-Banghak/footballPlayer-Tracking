# footballPlayer-Tracking
### *Team : I need a vacation* 


---
![ezgif com-video-to-gif (1)](https://github.com/We-Need-Banghak/footballPlayer-Tracking/assets/65584699/0e9fda69-6940-4fd8-8ecc-74e34fc3cf92)

## Dataset
* link: https://universe.roboflow.com/roboflow-jvuqo/football-players-detection-3zvbc/dataset/1


## Train 
1. Train Model - `YOLOv5`<br>

```python
!python train.py \
    --img 416 \
    --batch 16 \
    --epochs 70 \
    --data /content/drive/MyDrive/DL_AL_2/football-players-detection.v2i.yolov5pytorch_2/data.yaml \
    --cfg ./models/yolov5s.yaml \
    --weights yolov5s.pt \
    --name ball_yolov5s_result
```

## Detection 
1. Settings<br>
2. Set Custom annotator<br>
3. Detect Ball possession<br>
4. Get Ball Detection in Single Frame<br>
5. Get Full Video<br>
6. Full Video Tracking<br>
7. Final result

Base Decetcion|Ball possession detection|
|-----|-----|
|<img width="685" alt="img" src="https://github.com/We-Need-Banghak/footballPlayer-Tracking/assets/65584699/10d55cff-a986-4e65-b3f4-dd7e595e643b">|<img width="679" alt="img" src="https://github.com/We-Need-Banghak/footballPlayer-Tracking/assets/65584699/7e9078b2-e19a-4d74-bca6-60d12e2d2a59">|


## Directory structure

```bash
📦root
 ┣ 📂ByteTrack
 	┗..
 ┣ 📂clips
 	┗..
 ┣ 📂final
 	┗..
 ┣ 📂yolov5
 	┗..
 ┗ 📜best.pt
 ┗ 📜object_detection.py
```

## Using Libraries
- [YOLOv5](https://github.com/ultralytics/yolov5)
- [ByteTrack](https://github.com/ifzhang/ByteTrack.git)




### Members
* 202035369 이종은
* 202035525 서정덕
* 202035528 신수인
* 202035535 이지윤
