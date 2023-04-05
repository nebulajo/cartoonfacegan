# CartoonFaceGAN: A Study on Cartoon Face Generation Using Layer Swap, Distillation based StyleGAN2-ADA

[paper](https://drive.google.com/file/d/1bx59o9wM-2RqrmdMjPv0Ux68aVUH8Uu7/view)

Image to Image(I2I) Translation 이란 입력 이미지들을 특정 domain의 이미지로 변환하는 task이다. Input, Output 이미지들을 mapping 하는 것이 목적인 생성 모델 분야 중 하나이다. I2I 분야에서는 StyleGAN2-ADA 모델을 베이스
라인으로 사용하며, 이는 Mapping Network를 통해 Age, Gender, Smile과 같은 이미지의 Facial Attribute를 구분할 수 있다. 본 연구에서는 Cartoon 스타일을 적용한 StyleGAN2-ADA 기반의 얼굴 이미지 생성 모델을 제안한다. Layer Swap으로
실제 얼굴과 유사한 Cartoon 스타일의 얼굴 이미지를 생성하고, Distillation 기법을 활용하여, 순전파 방식으로 이미지의 Facial Attribute를 개별적으로 조정할 수 있다. 제안하는 방법론의 검증을 위해 네이버 웹툰 이미지를 데이터셋으로
구성하여, 기존의 StyleGAN2와 StyleGAN2-ADA로 전이학습한 결과와 실제 사람 이미지를 통해 비교 실험을 진행하 였으며, 제안하는 방법론의 우수성을 검증하였다.

## Architecture

<img width="607" alt="스크린샷 2023-04-01 오후 2 47 23" src="https://user-images.githubusercontent.com/126544082/229268059-773658b0-8b85-4727-8841-46dc5f4b160f.png">

본 논문에서는 실제 사람과 유사한 얼굴 이미지를 생성하는 Face Generation 연구를 수행하였다. StyleGAN2-ADA 모델에 Layer Swap 과 Distillation 을 적용한 CartoonFaceGAN 을 제안
하였다. 연구 결과 기존의 StyleGAN2 와 StyleGAN2-ADA 보다 실제 사람의 주름, 표정, 얼굴 형태와 같은 특징을 잘 반영하는 것을 확인하였다. 또한 Age, Gender, Smile 과 같은 Facial Attribute 를
개별적으로 자연스럽게 조정할 수 있는 것을 확인하였다.
