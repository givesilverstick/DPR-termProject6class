# DPR-termProject6class

케이크 이미지 6개 클래스를 분류하는 딥러닝 모델 프로젝트입니다.

![Unknown-2](https://github.com/givesilverstick/DPR-termProject6class/assets/108306340/8339ba36-0e7b-4ed8-9963-0b4d3bbee389)

[Colab 프로젝트 문서](https://colab.research.google.com/drive/1HGSJBJFHrHJMMFYPWKGTq05M9S849bOS?usp=sharing)

## 프로젝트 개요

이 저장소에는 케이크 이미지 분류 텀프로젝트에 필요한 다음 요소가 포함되어 있습니다.

- 클래스별로 정리된 학습/테스트 이미지 데이터셋
- 학습 완료된 모델 체크포인트
- 예측 실험에 사용한 테스트 이미지

## 분류 클래스

모델은 아래 6개 클래스를 분류합니다.

1. `carrot_cake`
2. `cheesecake`
3. `chocolate_cake`
4. `cup_cakes`
5. `red_velvet_cake`
6. `strawberry_shortcake`

## 데이터셋 구조

```text
train/
  <class_name>/*.jpg

test/
  <class_name>/*.jpg

cec_test_image/
  test*.png|jpeg
```

현재 저장소 기준 데이터셋 크기:

- Train: **4,506장**
- Test: **1,505장**

## 모델 산출물

사전 학습된 모델 파일이 포함되어 있습니다.

- `model/best_model_6class.hdf5`
- `model/cec_cake_classify_model.h5`
- `model/history.log`

## 빠른 시작 (Colab)

1. [Colab 프로젝트 문서](https://colab.research.google.com/drive/1HGSJBJFHrHJMMFYPWKGTq05M9S849bOS?usp=sharing)를 엽니다.
2. 필요 시 Google Drive를 마운트합니다.
3. 이 저장소 구조에 맞게 데이터셋 경로를 설정합니다.
4. 학습/평가/예측 셀을 순서대로 실행합니다.

## 추가 권장 사항 (선택)

프로젝트 재사용성과 협업 편의성을 높이기 위해 아래 항목을 추가하면 좋습니다.

- Python 패키지 의존성 파일 (`requirements.txt`)
- 학습 스크립트 (`train.py`) 및 추론 스크립트 (`predict.py`)
- 평가 지표 요약 (정확도, confusion matrix)
- 라이선스 정보
- 재현성 정보 (랜덤 시드, 이미지 크기, 데이터 증강 설정)
