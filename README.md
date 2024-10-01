# LoRA (Low-Rank Adaptation) from Scratch

이 저장소는 MNIST 데이터셋을 사용하여 LoRA (Low-Rank Adaptation) 기법을 실험한 내용을 담고 있습니다. / This repository contains an experiment using the LoRA (Low-Rank Adaptation) technique on the MNIST dataset.

## 프로젝트 개요 / Project Overview

이 프로젝트는 다음과 같은 실험을 수행합니다: / This project performs the following experiments:

1. 홀수 숫자만을 인식하도록 기본 신경망 모델을 학습 / Train a basic neural network model to recognize only odd numbers
2. LoRA Adapter를 추가하여 모든 숫자를 인식하도록 추가 학습 / Add LoRA Adapter to further train the model to recognize all numbers
3. 전체 파라미터의 약 1%만을 사용하여 95% 이상의 정확도 달성 / Achieve over 95% accuracy using only about 1% of the total parameters

## 주요 내용 / Main Contents

- `MNIST_LoRA_Experiment.ipynb`: 전체 실험 과정을 담은 Jupyter 노트북 / Jupyter notebook containing the entire experiment process
- 기본 MLP 모델 구현 / Implementation of basic MLP model
- LoRA Adapter 구현 및 적용 / Implementation and application of LoRA Adapter
- 모델 학습 및 평가 / Model training and evaluation
- LoRA 파라미터와 기본 모델의 병합 과정 / Merging process of LoRA parameters and base model

## 실험 결과 / Experiment Results

- 홀수만 학습한 기본 모델: 전체 데이터셋에 대해 약 50% 정확도 / Base model trained only on odd numbers: About 50% accuracy on the entire dataset
- LoRA 적용 후 모델: 전체 데이터셋에 대해 95% 이상의 정확도 / Model after applying LoRA: Over 95% accuracy on the entire dataset
- 사용된 학습 가능 파라미터: 전체의 약 2.37% / Trainable parameters used: About 2.37% of the total
- LoRA 파라미터와 기본 모델을 성공적으로 병합하여 전체 데이터셋에 대해 96.78%의 정확도 달성 / Successfully merged LoRA parameters with the base model, achieving 96.78% accuracy on the entire dataset

## 참고 자료 / References

- [LoRA: Low-Rank Adaptation of Large Language Models](https://arxiv.org/abs/2106.09685)

## 라이센스 / License

이 프로젝트는 MIT 라이센스 하에 배포됩니다. 자세한 내용은 `LICENSE` 파일을 참조하세요. / This project is distributed under the MIT License. See the `LICENSE` file for more details.
