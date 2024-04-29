# 주변 환경 소리 분석
1. [분리](#분리)
2. [분류](#분류)
---
# 분리
주변 환경의 중첩된 소리를 단일 소리로 분리

## Demucs
[Demucs](https://github.com/facebookresearch/demucs) is a music source separation model that supports drum, bass, and vocal separation based on U-Net convolutional architecture.

하나의 input 파일당 4개의 output 파일을 생성한다.

---
# 분류
각각의 단일 소리를 분석해 어떤 소리인지 분류

## Dataset
ESC-50, AI-Hub 소음 환경 음성인식 데이터, UrbanSound8K

+ __630개의 데이터__
  + Train Data 513개
  + Validation Data 117개

+ __11개의 카테고리__
  + dog
  + cat
  + rain
  + wind
  + thunderstorm
  + human
  + conversation
  + siren
  + car horn
  + train
  + steet_music

## ResNet-34
분리된 음성 데이터를 분류하기 위해 PyTorch RESNET34 이용

## 데이터 전처리
+ __def spec_to_image__

오디오 스펙트로그램을 받아서 이미지로 변환
　　　　　

# Members
|<img src="https://avatars.githubusercontent.com/u/108173863?v=4" width="150" height="150"/>|<img src="https://avatars.githubusercontent.com/u/98511311?v=4" width="150" height="150"/>|
|:-:|:-:|
|Hyeonji Roh<br/>[@hyeonjiroh](https://github.com/hyeonjiroh)|Yunju Nam<br/>[@SouthYunnnn](https://github.com/SouthYunnnn)|
