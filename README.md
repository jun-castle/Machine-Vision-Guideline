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
  - [About Edge Detection❓🎯 ](#about-edge-detection)

  - [About Class Imbalance and Data Augmentation❓🎯 ](#about-class-imbalance-and-data-augmentation)
  - [About Deep Learning with GAN❓🎯 ](#about-deep-learning-with-gan)
  - [About OCR❓🎯 ](#about-ocr)



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

## About Edge Detection❓🎯
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

## About Class Imbalance and Data Augmentation❓🎯
  ### **1) class Imbalance**
  <p align="center">
  <img src="https://github.com/user-attachments/assets/7feb3b33-f8e6-49f2-ab49-24344157a95a" width="550" height="auto" alt="5">
  </p>
  - 학습 편향 및 모델 성능 저하:<br />
 불량 사례(소수 클래스)에 비해 정상 사례(다수 클래스)의 데이터가 지나치게 많으면 모델이 다수 클래스에 치우쳐 학습됩니다. 이 경우, 모델은 대부분 정상으로 예측하여 의도와 다르게 불량을 놓치는 경향이 커집니다.<br />
  - 평가 및 검증의 문제:<br />
 불균형 데이터에서는 정확도만으로 성능을 평가하면 안 됩니다. 정밀도(Precision), 재현율(Recall), F1 스코어, ROC AUC 등 소수 클래스에 민감한 지표를 함께 고려해야 합니다. 또한 불균형이 검증 셋에도 동일하게 적용되면, 모델 평가 시 불량 탐지 성능을 제대로 반영하지 못할 수 있습니다. 따라서 클래스 비율을 고려한 적절한 검증 전략이 필요합니다.<br />
  - 학습 과정 및 최적화의 어려움:<br />
 표준 손실 함수(예: 크로스 엔트로피)는 다수 클래스 데이터에 의해 주도되어 소수 클래스의 학습에 소홀해질 수 있습니다. 이로 인해 불량 탐지 성능이 떨어질 수 있습니다. 학습 시 불균형 데이터로 인해 모델이 단순히 다수 클래스를 예측하는 트릭(Trivial solution)에 빠져 버릴 위험이 있습니다. 또한 SMOTE와 같은 오버샘플링 기법은 소수 클래스 데이터를 인위적으로 증강하지만, 이로 인해 과적합(overfitting) 문제가 발생할 수 있습니다. 즉, 모델이 특정 불량 샘플에 지나치게 최적화되어 일반화 능력이 저하될 수 있습니다.<br />
<br />
 
 이와 같은 문제들을 완화하기 위한 방법으로 아래 예시들이 있습니다.<br />
 * 데이터 증강 및 합성 샘플 생성:<br />
   데이터 증강 또는 GAN 등의 생성모델을 통한 합성 샘플 생성<br />
 * 클래스 가중치 조정:<br />
   손실함수에 클래스별 가중치를 부여하거나 Focal loss와 같은 기법을 사용하여 소수 클래스에 집중하도록 학습 유도<br />
 * Anomaly detection기반 접근론:<br />
   불량 데이터가 극히 드물다면, 지도학습 대신 비지도학습이나 준지도학습 기반의 이상 탐지 방법을 고려 가능<br />


  ### **2) Data Augmentation**
  <p align="center">
  <img src="https://github.com/user-attachments/assets/d90eef20-41db-4b42-9889-2686ffa9e7e0" width="550" height="auto" alt="6">
  </p>
   데이터를 확보하기 위한 증강 과정에서도 데이터의 특징을을 고려해야 한다. 만약에 취득된 이미지가 모두 같은 위치의 제품을 촬영한 것이 아니라 아래와 같은 요인들의 영향을 받는다면, 데이터 증강을 통해서 기존 데이터로 새로운 데이터 확보를 하는 처리에서 이를 반영해야 합니다.<br />

   
  * 회전<br />
  : 다양한 각도에서 촬영된 제품 이미지를 확보하여 학습함으로서 다양한 각도에 대한 모델의 일반화된 인식 능력을 향상시킵니다.<br />
  * 빛 번짐<br />
  : 조명 변화와 빛 번짐 효과를 모방하기 위해 이미지의 밝기, 대비, 채도 등을 조절하거나 가우시안 블러(gaussian blur)와 같은 필터를 적용합니다.<br />
  * 스케일<br />
  : 모델이 다양한 거리에서 촬영된 제품을 인식하도록 합니다.<br />
  * 평행이동<br />
  : 이미지를 수평 또는 수직 방향으로 이동시켜 제품이 이미지 내 다양한 위치에 나타나는 상황을 만듭니다.<br />
  * 반전<br />
  : 이미지의 좌우 또는 상하 반전을 수행합니다. 또한, 색상 반전 등도 고려할 수 있습니다.<br />
   


## About Deep Learning with GAN❓🎯
  <p align="center">
  <img src="https://github.com/user-attachments/assets/aa7b1a60-3f41-4884-a22d-0a4583ca94ce" width="550" height="auto" alt="7">
  </p>
   재구성(Reconstruction) 및 생성(Generation) 기반 이상탐지는 데이터 불균형이 큰 상황에서 정상 데이터만을 학습하여 이를 바탕으로 비정상 데이터를 탐지하는 기법입니다. U-Net과 같은 구조의 네트워크를 사용하여 입력 데이터를 압축(인코딩)하고 다시 복원(디코딩)합니다. 단, 학습이 정상 데이터만으로 이루어지기 때문에 이를 통해 아래와 같은 효과를 기대한다고 할 수 있습니다.<br />

  <원리>
   * Normal Data (정상 데이터):<br />
   : 학습 과정에서 충분히 익힌 패턴을 따르는 데이터의 경우에는 모델이 해당 데이터를 높은 품질로 잘 재구성할 수 있습니다.<br />
   * Abnormal Data (비정상 데이터):<br />
   : 학습하지 않은 패턴을 따르는 이상치가 입력될 경우, 모델이 이를 재구성하는 데 어려움을 겪어 원본과 큰 차이를 보일 수 있습니다. 따라서 정상 데이터에 비해 재구성 과정의 오류가 클 것이므로 이를 통해 abnomaly score를 정량화하여 비정상으로 판별할 수 있게 됩니다.<br />


  <고려사항>
  * 학습 안정성<br />
  : GAN과 같은 경우 학습이 불안정할 수 있으며, 해당 경우 적절한 하이퍼파라미터 튜닝과 설계가 필요합니다.<br />
  * 계산 비용<br />
  : 잠재 공간 최적화 과정(AnoGAN)은 계산 비용이 높을 수 있습니다. 실시간 이상 탐지에는 최적화가 필요할 수 있습니다.<br />
  * 데이터의 다양성<br />
  : 정상 데이터만을 가지고 비지도 학습을 거치기 때문에 학습 데이터의 범위가 충분히 넓어야 실제 환경에서 다양한 정상 사례를 모두 포괄하여 이상 탐지 정확도를 높일 수 있습니다.<br />


  
## About OCR❓🎯
  ### 1. 텍스트 인식과 일반 이미지 인식의 차이점
  * 구조적 특성<br />
  : 일반 이미지 인식은 다양한 객체, 배경, 색상, 질감 등을 포괄하는 반면, 텍스트 인식은 글자와 단어의 형태, 서체, 배열 등에 집중합니다.<br />
  * 공간적 관계<br />
  : 일반 이미지에서는 객체 간 관계와 장면 구성이 중요하지만, 텍스트 인식은 연속된 문자 패턴과 단어의 배열에 중점을 둡니다.<br />
  ### 2. 텍스트 유사도 측정의 특수성
  * 문자 기반 비교<br />
  : 텍스트 유사도 측정은 픽셀 단위 비교가 아닌, 문자와 단어 수준의 편집 거리(Levenshtein distance), Jaccard 유사도, 코사인 유사도 등의 문자열 기반 방법을 사용합니다.<br />
  * 구조적 및 시각적 특징 고려<br />
  : 텍스트 이미지에서는 글자 모양, 서체, 크기, 글자 간격 등의 구조적 특징이 중요합니다. 따라서 단순히 문자열 비교뿐만 아니라, 이미지 내 문자 패턴의 구조적 유사성 분석이 필요합니다.<br />
  * 문맥 이해와 의미론적 비교<br />
  : 경우에 따라 텍스트의 문맥이나 의미적 유사성을 고려하기 위해 자연어 처리 기법을 접목하여, 오타나 비슷한 모양의 문자를 문맥상에서 평가하기도 합니다.<br />

  ### 3. OCR 소개
  <p align="center">
  <img src="https://github.com/user-attachments/assets/d756dc62-6d83-46bb-b7bb-69050d4b9894" width="550" height="auto" alt="8">
  </p>
   OCR(Optical Character Recognition)은 이미지나 스캔 문서 내의 텍스트를 인식하여 기계가 읽을 수 있는 문자 데이터로 변환하는 기술입니다.
  * 소개<br />
  : OCR 시스템은 먼저 이미지 내 텍스트 영역을 검출하고, 각 문자를 개별적으로 분할한 후, 문자 인식 알고리즘(예: 딥러닝 기반 CNN, RNN 등)을 통해 문자를 식별합니다. 이후 인식된 문자들을 조합하여 단어와 문장으로 구성합니다. OCR은 문서 디지털화, 자동 번호판 인식, 의료 기록 처리, 금융 서류 분석 등 다양한 분야에서 활용되고 있습니다.<br />
 
  ### 4. OCR의 한계점
  * 언어 및 서체 다양성<br />
  : 다양한 언어, 복잡한 서체, 손글씨 등에 대해 OCR 인식률이 낮을 수 있습니다. 특정 언어나 특수 서체에 대한 학습 데이터 부족이 원인이 될 수 있습니다.<br />
  * 노이즈와 품질 저하<br />
  : 미지가 흐릿하거나 노이즈, 왜곡, 배경과의 대비 부족 등의 문제로 인해 인식 정확도가 떨어질 수 있습니다. 조명 조건이나 촬영 각도에 의한 품질 저하도 OCR 성능에 영향을 줍니다.<br />
  * 레이아웃 및 복잡한 배경<br />
  : 복잡한 배경이나 다양한 레이아웃에서 텍스트를 정확히 검출하고 인식하는 것이 어려울 수 있습니다. 특히 자연 환경 사진 속의 텍스트 인식은 많은 도전 과제를 안고 있습니다.<br />
  * 실시간 처리 성능<br />
  : 고속 실시간 텍스트 인식이 필요한 응용에서는 OCR의 처리 속도와 정확도 사이에서 균형을 맞추는 것이 중요한 쟁점이 될 수 있습니다.<br />
  * 복원 불가능한 손상<br />
  : 고속 실시간 텍스트 인식이 필요한 응용에서는 OCR의 처리 속도와 정확도 사이에서 균형을 맞추는 것이 중요한 과제입니다.<br />


 이와 같이 텍스트 인식 분야는 일반 이미지 인식과 차별화되는 특성과 유사도 측정 방법을 가지며, OCR 기술은 다양한 응용 가능성을 제공하지만 여러 한계점도 존재합니다. 연구와 기술 발전을 통해 이러한 한계점을 극복하고 더 정확하고 범용적인 텍스트 인식 시스템을 구축하기 위한 노력이 지속되고 있습니다.
