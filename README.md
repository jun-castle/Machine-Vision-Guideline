<p align="center">
<img src="https://capsule-render.vercel.app/api?type=rounded&color=A3DCBE&height=200&section=header&text=Guideline%20for%20Machine%20Vision&fontSize=50" />
</p>

<p align="center">
<img src="https://img.shields.io/badge/python-%233776AB.svg?&style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/pytorch-%23EE4C2C.svg?&style=for-the-badge&logo=pytorch&logoColor=white" />
</p>


## 🛠 Contents (❓:Concept / 🎯: Application)
  - [About Machine Vision❓ ](#about-Machine-Vision)
  - [About Template Matching❓ ](#about-Template-Matching)
  - [Template Matching 기반으로 image를 crop하기 🎯 ](#template-matching-기반으로-image를-crop하기)
  - [About Edge Detection❓ ](#about-edge-detection)

  - [About Class Imbalance and Data Augmentation❓ ](#about-class-imbalance-and-data-augmentation)
  - [About Deep Learning with CNN❓ ](#about-deep-learning-with-cnn)
  - [About GradCAM❓ ](#about-gradcam)



## About Machine Vision❓
  <p align="center">
  <img src="https://github.com/user-attachments/assets/af0011c4-2f76-4248-8fea-e18f565d2c83" width="450" height="auto" alt="1">
  </p>

  머신비전(Machine Vision)은 컴퓨터가 카메라와 이미지 처리 기술을 이용해 시각적 정보를 획득, 분석, 이해하여 인간의 시각적 판단을 모방하거나 대체하는 기술입니다. 이는 자동화 공정, 품질 검사, 로봇 제어 등 다양한 산업 분야에서 활용됩니다.
  
  ### 머신비전의 주요 구성 요소
  - **이미지 획득**: 카메라나 센서를 이용해 대상의 디지털 이미지를 캡처합니다.
  - **이미지 처리**: 획득한 이미지를 전처리(노이즈 제거, 보정 등)하고 분석할 수 있는 형태로 가공합니다.
  - **특징 추출 및 분석**: 이미지에서 유의미한 패턴이나 객체를 인식하고 분류하여 원하는 정보를 추출합니다.
  - **결정 및 제어**: 분석 결과를 바탕으로 자동화 시스템에 피드백을 제공하거나 제어 명령을 내립니다.
  
  ### 머신비전과 딥러닝, 머신러닝
  머신비전 분야에서는 최근 딥러닝과 머신러닝 기술이 중요한 역할을 하고 있습니다. 
  - **머신러닝**: 과거의 데이터로부터 학습하여 패턴을 인식하거나 예측하는 기술. 전통적인 이미지 처리 기법에서 특징 추출 및 분류에 활용됩니다.
  - **딥러닝**: 인공신경망을 이용해 복잡한 이미지 패턴을 자동으로 학습하고 인식하는 방법. 특히 컨볼루션 신경망(CNN)은 이미지 분류, 객체 검출, 세분화 등에 뛰어난 성능을 보이며, 머신비전에서 많이 사용됩니다.
  
  딥러닝 기반의 머신비전은 작업자가 포착하기 어려운 복잡한 패턴이나 변형에 대해서도 높은 정확도로 인식하고 분석할 수 있으며 더불어 자동화 공정의 효율성과 정확성을 크게 향상시킵니다.
  
  ### 머신비전의 응용 분야
  - **품질 검사**: 생산 라인의 제품을 실시간으로 검사하여 불량품을 자동으로 선별
  - **로봇 제어**: 로봇이 시각 정보를 바탕으로 물체를 인식하고 조작
  - **자동화 공정**: 카메라와 센서를 통해 공정 상태를 모니터링하고 이상을 감지하여 자동으로 조정
  - **의료 영상 분석**: 의료 이미지를 분석해 질병 진단 지원

## About Template Matching❓ 
  <p align="center">
  <img src="https://github.com/user-attachments/assets/967c8cc0-33b1-48df-b31b-73035d59fc57" width="450" height="auto" alt="2">
  </p>
   Template matching은 원본 이미지에서 내가 찾고자 하는 부분(template image)를 찾는 기법이다. 원본 이미지 위에서 탬플릿 이미지를 이동시켜 가면서 탬플릿 이미지와 동일하거나 가장 유사한 영역을 찾는다. 원본 이미지와 탬플릿 이미지의 크기는 같을 필요가 없다. 단, 원본 이미지가 회전되어 있는 경우에는 인식력이 떨어질 수 있다는 단점이 있다.

## Template Matching 기반으로 image를 crop하기🎯 
  <p align="center">
  <img src="https://github.com/user-attachments/assets/30516582-5414-493b-93f7-736ff675adc0" width="450" height="auto" alt="3">
  </p>

  * Step 1. 원본 이미지에서 template image와 가장 유사한 부분을 인식<br />
  * Step 2. 인식된 부분의 중심 픽셀 위치 기준으로 원본 이미지에서 *ROI만 남기도록 crop

  \* ROI: Region Of Interest (관심영역)

## About Edge Detection❓
  <p align="center">
  <img src="https://github.com/user-attachments/assets/4d0697ee-45fe-4c5c-8ae8-ed4bdc8fd3e5" width="550" height="auto" alt="4">
  </p>
   Canny Edge Detection은 이미지의 가장자리(Edge)를 감지하는 데 사용되는 edge detection 알고리즘으로서 작은 오류로 edge map을 생성하는 최적의 알고리즘으로 평가 받으며 다양한 머신 비전 어플리케이션에서 전처리 단계로 활용될 수 있습니다..<br />
   자율 주행 차량에서 도로 차선 또는 도로 경계를 검출하는 데에 이용되어 차선 유지나 차선 변경 보조 등의 구현이 가능합니다. 또한 생산 라인 이후 제품의 크랙 또는 흠집과 같은 결함을 검출하는 데에 이용되어 자동 품질 검사 시스템에서 사용될 수 있습니다.<br />
   
  * Step 1. 노이즈 제거<br />
    : Edge 검출 전 이미지에 내제하는 노이즈를 줄이기 위해 가우시안 필터를 이용하여 노이즈를 제거하여 이미지를 좀 더 부드럽게 처리합니다.<br />
  * Step 2. 그래디언트 계산<br />
    : Sobel 등의 미분 필터를 사용해 각 픽셀에서의 주변 픽셀 간의 기울기를 계산하는 과정에서 픽셀 간 edge 강도(gradient magnitude)와 방향(gradient direction)을 얻습니다.<br />
  * Step 3. 비최대 억제 (Non-maximum Suppression)<br />
    : 계산된 그래디언트 정보를 바탕으로 edge 픽셀만 남기고 주변 픽셀은 억제하여 edge가 얇고 선명하게 추출되도록 합니다.<br />
  * Step 4. 이중 임계값 적용 (Double Thresholding)<br />
    : 비최대 억제 후 남은 픽셀들에 대해서 높은 임계값과 낮은 임계값을 적용합니다. Strong edge는 높은 임계값을 넘고, weak edge는 낮은 임계값만을 넘는 픽셀로 구분됩니다.<br />
  * Step 5. 엣지 추적 (Edge Tracking by Hysteresis)<br />
    : Weak edge가 실제 edge의 연장선인지 확인하기 위해서 strong edge와 연결되어 있는지 검사합니다. Strong edge와 연결되어 있는 weak edge는 최종 검출되는 edge에 포함시키고 그렇지 않은 weak edge는 제거합니다.<br />

## About Class Imbalance and Data Augmentation❓ 
  ### **1) class Imbalance**
  <p align="center">
  <img src="https://github.com/user-attachments/assets/7feb3b33-f8e6-49f2-ab49-24344157a95a" width="550" height="auto" alt="5">
  </p>
  - 학습 편향 및 모델 성능 저하: 불량 사례(소수 클래스)에 비해 정상 사례(다수 클래스)의 데이터가 지나치게 많으면 모델이 다수 클래스에 치우쳐 학습됩니다. 이 경우, 모델은 대부분 정상으로 예측하여 의도와 다르게 불량을 놓치는 경향이 커집니다.
  - 평가 및 검증의 문제: 불균형 데이터에서는 정확도만으로 성능을 평가하면 안 됩니다. 정밀도(Precision), 재현율(Recall), F1 스코어, ROC AUC 등 소수 클래스에 민감한 지표를 함께 고려해야 합니다. 또한 불균형이 검증 셋에도 동일하게 적용되면, 모델 평가 시 불량 탐지 성능을 제대로 반영하지 못할 수 있습니다. 따라서 클래스 비율을 고려한 적절한 검증 전략이 필요합니다.
  - 학습 과정 및 최적화의 어려움: 표준 손실 함수(예: 크로스 엔트로피)는 다수 클래스 데이터에 의해 주도되어 소수 클래스의 학습에 소홀해질 수 있습니다. 이로 인해 불량 탐지 성능이 떨어질 수 있습니다. 학습 시 불균형 데이터로 인해 모델이 단순히 다수 클래스를 예측하는 트릭(Trivial solution)에 빠져 버릴 위험이 있습니다. 또한 SMOTE와 같은 오버샘플링 기법은 소수 클래스 데이터를 인위적으로 증강하지만, 이로 인해 과적합(overfitting) 문제가 발생할 수 있습니다. 즉, 모델이 특정 불량 샘플에 지나치게 최적화되어 일반화 능력이 저하될 수 있습니다.

  
## About Deep Learning with GAN❓ 


## About GradCAM❓ 


