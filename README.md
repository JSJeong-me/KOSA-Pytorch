# KOSA-Pytorch

# KOSA-Python과 Pytorch를 활용한 인공지능 딥러닝 입문과정

## 강사: 정 준 수 Ph.D (heinem@naver.com)

### 교육목표
### 딥러닝의 원리를 이해하고 Pytorch의 다양한 라이브러리를 인공지능 모델개발에 적용

	1일차 [딥러닝 모델]
	
  - 딥러닝 도구 및 모델의 종류 이해
  - 환경 설정 방법 및 도구 활용 방법 소개
  - Neural Network 작동 원리 및 딥러닝 모델 개요
  - 경사하강법 및 역전파 알고리즘 이해
  - Numpy crash - 시각화 도구 (Matplotlib) crash
  - Pytorch 주요 라이브러리 소개 - 연습문제 및 실습
 	
	2일차 [딥러닝 모델]
	
  - 딥러닝을 위한 데이터 준비 및 모델 적용 후 성능 검증
  - Activation Function 및 Hyper Parameter 설정 이해
  - Neural Network Regression Model 구현
  - Housing Price 예측 모델 실습 - 딥러닝 Classification Model 구현
  - MNIST Dataset을 통한 손글씨 인식 실습
  - Hyper-parameter 조정을 통한 모델 성능 개선
  - 연습 문제 및 실습

	3일차 [딥러닝 모델]
	
  - 이미지 인식 model 과 Layers API 이용
  - Convolutional N.N 알고리즘 이해
  - Image 특성 추출 kernel 작동 원리 이해
  - Le Net 구축을 통한 이미지 인식 모델 
  - Image Generator API를 활용한 Train/Validation data 구조화
  - pre-trained model 의 학습 전이 기능 이해
  - 모델 성능 평가 - 연습문제 및 실습

  	4일차 [딥러닝 모델]
	
  - 자연어 인식 모델과 시계열 데이터 학습 모델 구현
  - Sequence Model 이해 - RNN 및 LSTM 알고리즘 이해
  - Language Model 소개 및 작동 알고리즘 이해
  - RNN 모델을 이용한 감성분석 - 자연어 처리 모델 소개
  - Auto-encoder 모델 소개 - wrap-up 및 평가



Advanced TensorFlow users familiar with “GradientTape” know that it takes significantly more code to train a network than simply calling “model.fit”, but the additional control you have is sometimes worth it, especially if you are doing state-of-the-art research.

Thus, you think of PyTorch as being in “GradientTape” mode by default — the training loop must be implemented by hand which will require additional code.

My thoughts: Yes, coding neural networks and training procedures with PyTorch does take more code, and oftentimes more effort than the higher-level Keras API; however, Keras doesn’t give you control over what happens inside “model.fit” — PyTorch does.

Yes, but: All that flexibility comes at a cost though. I haven’t met a single deep learning practitioner who hasn’t at least once screwed up:

Zeroing their gradients with “opt.zero_grad()”
Performing backpropagation with “loss.backward()”
Updating their model weights with “opt.step()”
