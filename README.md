# vision-ai

> 비전AI와비즈니스(2026-2) 주차별 실습 — Hugging Face 모델로 객체 검출·세분화 등 비전 AI 실험 (Colab T4)

매주 Hugging Face 모델로 진행한 비전 AI 실습 코드와 결과를 정리한 저장소입니다.
모든 실습은 **Google Colab (T4 GPU)** 에서 실행했으며, 노트북을 열고 `런타임 > 모두 실행`으로 재현할 수 있습니다.

## 주차별 실습

| 주차 | Task | 모델 (Hugging Face) | 데이터 | 핵심 결과 | 노트북 |
|---|---|---|---|---|---|
| 5주차 | 객체 검출 (Object Detection) | RT-DETR-R18, DETR-R50, YOLOS-tiny | COCO val2017 (200장) | RT-DETR mAP 0.495 / 19.6 FPS | [object_detection.ipynb](week05_object-detection/object_detection.ipynb) |
| 6주차 | 세분화 (Segmentation) | U-Net, SegFormer-B0, SAM | Oxford-IIIT Pet | (작성 예정) | [segmentation.ipynb](week06_segmentation/segmentation.ipynb) |

## 폴더 구조

```
vision-ai/
├── README.md                 ← 지금 이 파일 (전체 목차)
├── requirements.txt
├── .gitignore                ← 데이터·가중치·zip은 제외
├── week05_object-detection/
│   ├── README.md             ← 주차별 요약 (목표·모델·결과·배운 점)
│   ├── object_detection.ipynb
│   └── results/              ← results.json, 결과 그림(png)
└── week06_segmentation/
    ├── README.md
    ├── segmentation.ipynb
    └── results/
```

## 실행 환경
- Google Colab, NVIDIA Tesla T4 GPU
- PyTorch, Hugging Face Transformers (버전은 각 주차 `results/results.json`의 `env` 참고)
