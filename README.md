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

  - [About PCA❓ ](#about-PCA)
  - [About Data Augmentation❓ ](#About-Data-Augmentation)
  - [About Deep Learning with CNN❓ ](#About-Deep-Learning-with-CNN)
  - [About GradCAM❓ ](#About-GradCAM)



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
   Canny Edge Detection은 이미지의 가장자리(Edge)를 감지하는 데 사용되는 edge detection 알고리즘으로서 작은 오류로 edge map을 생성하는 최적의 알고리즘으로 평가 받는다.<br />
   자율 주행 차량에서 도로 차선 또는 도로 경계를 검출하는 데에 이용되어 차선 유지나 차선 변경 보조 등의 구현이 가능합니다. 또한 생산 라인 이후 제품의 크랙 또는 흠집과 같은 결함을 검출하는 데에 이용되어 자동 품질 검사 시스템에서 사용될 수 있습니다.<br />
   
  * Step 1.<br />
  * Step 2.<br />
  * Step 3.<br />
  * Step 4.<br />
  * Step 5.

## About PCA❓ 
## About Data Augmentation❓ 
## About Deep Learning with CNN❓ 
## About GradCAM❓ 


