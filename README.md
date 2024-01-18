# ML-MoS2-defect-detect
MoS2 (이황화 몰리브데늄)을 촬영한 STEM 이미지상에 나타난 Sulfur defects를 감지하는 머신러닝 모델을 제작했습니다. 
<br/>
<br/>
🔗 레퍼런스: [STEM Image Analysis Based on Deep Learning: Identification of Vacancy Defects and Polymorphs of MoS2](https://pubs.acs.org/doi/10.1021/acs.nanolett.2c00550)

🔗 레퍼런스: [Generating STEM Simulated Image](https://github.com/Chuqiao2333/STEM-Simulation-Images)


<br/>

# Introduction
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/a78e7e46-e2be-487a-968b-c3fa1bb96199)
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/25c8fbd9-efaa-4c25-a17a-2c13a9a51e10)

<br/>


# Architecture
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/7f52dd2e-2678-418c-9bc0-fa32b652d3d6)
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/b3207bfe-dbb6-447b-be57-ead6c1cb9a56)

<br/>


# Generating Training Set
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/edc22f62-c7a9-42f9-901c-019f9cb159c9)


<br/>


# Training
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/9074a5d1-97c9-4da9-8d97-ebad7ad448f4)

<br/>

# Crop Augmentation의 효과: Augmentation I vs Augmentation II
- Augmentation I: w/ Crop Augmentation
- Augmentation II w/o Crop Augmentation
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/72305954-d2b0-46e7-885f-85726389b3a3)

<br/>

## Case1: Predict Region: 5x5nm
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/ea2cb877-dbb7-4d8a-a759-8350c710562a)\

<br/>

## Case2: Predict Region: 2.5x2.5nm
crop augmentation 과정을 거치지 않은 Training Set으로 훈련시킨 모델의 경우 2.5x2.5nm 영역에 대한 예측성능이 상대적으로 낮다는 것을 확인할 수 있었습니다. 
<br/>
![image](https://github.com/sozign/ML-MoS2-defect-detect/assets/148179726/fa71acd8-9b95-46cc-9aae-bc517b062182)

