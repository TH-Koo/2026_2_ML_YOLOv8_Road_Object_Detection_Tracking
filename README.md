# YOLOv8 기반 도로 객체 탐지 및 추적

2026-2 머신러닝

자율주행의 주변 환경 인식을 주제로, YOLOv8을 학습하여 도로 영상의 객체를 탐지하고 BoT-SORT로 추적합니다.

## 탐지 대상

- **person**: 사람
- **vehicle**: 승용차, 버스, 트럭
- **traffic_sign**: 도로 표지판

## 데이터셋 및 개발 환경

- 데이터셋: [BDD100K YOLO Format](https://www.kaggle.com/datasets/a7madmostafa/bdd100k-yolo)
- 원본 라벨을 위의 3개 부류로 재구성하여 학습
- 개발 환경: Python, PyTorch, Ultralytics YOLOv8, Google Colab
- 추적 알고리즘: BoT-SORT

## 실행 순서

1. Google Colab에서 노트북을 엽니다.
2. GPU 런타임을 선택합니다.
3. 데이터 다운로드 및 라벨 변환 셀을 실행합니다.
4. YOLOv8 학습을 진행합니다.
5. 도로 영상을 업로드하고 객체 탐지·추적을 실행합니다.
6. 결과 영상을 MP4로 저장합니다.

결과 영상에는 객체의 경계상자, 클래스 이름, 추적 ID가 표시됩니다.
