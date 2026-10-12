# 6주차 — 세분화 (Segmentation) 실습

## 목표
강의에서 다룬 **클래식 전용 학습 모델(U-Net)** 과 **파운데이션 모델(SAM)** 을 같은 데이터에서 비교한다.
"전용 정밀 작업은 U-Net, 범용·빠른 적용은 SAM"이라는 강의 내용을 실험으로 확인한다.

## 실험 구성
- **모델**
  - U-Net (ResNet34 인코더, ImageNet 사전학습) — 파인튜닝
  - SegFormer-B0 (`nvidia/mit-b0`) — 파인튜닝
  - SAM (`facebook/sam-vit-base`) — 재학습 없이 박스/점 프롬프트로 zero-shot
- **데이터**: Oxford-IIIT Pet (반려동물 전경/배경 이진 분할) — 학습 1,000 / 검증 200 / 테스트 300장, 256×256
- **평가**: IoU, Dice (픽셀 단위)

## 결과
(실행 후 작성)
