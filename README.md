# MMDetection 3.3.0 Inference Code

**MMDetection 3.3.0** 버전에서 학습된 모델을 이용해 이미지를 inference할 때 사용할 수 있는 코드를 만들어봤다.

코드를 실행하면 모델이 예측한 값들이 (e.g., labels, bounding box information, confidence score, etc) 해당 이미지 파일과 동일한 이름을 가진 csv 파일들과 detection 결과 이미지들이 생성된다.

# Usage

```
python inference.py \
work_dirs/deformable-detr_r50_16xb2-50e_coco/deformable-detr_r50_16xb2-50e_coco.py(config file path) \
work_dirs/deformable-detr_r50_16xb2-50e_coco/ddetr_ev_epoch_470.pth(checkpoint file path) \
--inference_path <Inference Image path> \
--out_dir <result path>
```

# Reference
https://github.com/open-mmlab/mmdetection

https://mmdetection.readthedocs.io/en/latest/get_started.html
