---
layout: page
title: 방법론(Method)의 Technical Soundness를 강화하기 위한 본론 작성 방법
permalink: /lecture/material/intro-technical-writing/method
image: CUK_4Seasons.jpg
description: 논문에서 본론(Method 파트)는 연구의 핵심 아이디어와 기술적 구현을 설득력 있게 설명하는 심장부라고 해도 과언이 아닙니다. 기술적 타당성(Technical Soundness)이란, 간단히 말해 “이 방법이 정말 맞는 방법인가?”에 대한 이론적·실험적 근거와 논리를 탄탄히 깔아두는 것을 의미합니다.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

논문에서 **본론(Method 파트)**는 연구의 **핵심 아이디어**와 **기술적 구현**을 설득력 있게 설명하는 **심장부**라고 해도 과언이 아닙니다.  
**기술적 타당성(Technical Soundness)**이란, 간단히 말해 **“이 방법이 정말 맞는 방법인가?”**에 대한 이론적·실험적 근거와 논리를 탄탄히 깔아두는 것을 의미합니다.

- **AI 학회 심사** 시, 이 부분에서 ‘알고리즘의 논리적 결함’, ‘실험 설정이 불충분’, ‘설명 불명확’ 등의 지적을 받으면 **Reject** 확률이 급격히 높아집니다.  
- 따라서 **본론(Method)**을 작성할 때는 **수식, 알고리즘 단계, 모델 구조, 구현 세부사항** 등을 **체계적으로 명료하게** 풀어내야 합니다.

---

## 1. 왜 Method(본론)가 중요한가?

1. **연구 가치의 결정적 증거**  
   - AI 논문의 서론이나 Related Work에서 “이 문제가 중요하다”를 아무리 주장해도, **본론에서 제시하는 해결책**이 부실하면 연구 자체가 설득력을 잃습니다.

2. **재현 가능성(Replicability)**  
   - AI 연구는 **재현 가능성**이 매우 중요한 화두입니다. 심사위원이나 후속 연구자가 “이 방법을 똑같이 구현해볼 수 있나?”를 판단하기 위해 Method 파트를 꼼꼼히 봅니다.

3. **기술적 기여**  
   - “어떤 혁신적인 모델 구조를 제시하는가?”, “어떤 수학적 기여(정리, 증명)를 추가했는가?”, “어떤 성능 최적화나 메모리 개선 방법을 쓰는가?” 등이 **본론**에서 드러나야 합니다.

---

## 2. 본론(Method) 섹션 구성

AI 논문에서 Method 파트는 보통 아래와 같이 세분화할 수 있습니다:

1. **Overview of the Proposed Method**  
   - 제안 접근법의 **큰 그림**을 먼저 보여줍니다(예: 시스템 다이어그램, 알고리즘 흐름도, 모델 구조 그림 등).

2. **Details of Model/Algorithm**  
   - 수식(수학적 공식), 네트워크 아키텍처(레이어 구조), 알고리즘 단계를 구체적으로 설명  
   - 필요하다면, 서브 섹션(2.1, 2.2 …)으로 쪼개서 **핵심 아이디어**와 **보조 기법(Regularization, Optimization Trick 등)**을 구분

3. **Implementation / Training Setup**  
   - 실제 학습 환경(GPU, 프레임워크), 하이퍼파라미터 설정(학습률, 배치 사이즈 등)  
   - 모델이 얼마나 복잡한지(파라미터 수), 각 단계에 어떤 라이브러리를 썼는지 등

4. **Complexity & Theoretical Analysis (Optional)**  
   - 가능하다면 시간 복잡도, 공간 복잡도, 혹은 **이론적 안정성/수렴성 증명** 등을 제시  
   - 탑티어 학회에서는 이론적 분석이 있으면 가점을 받을 수 있음

(각 AI 학회/저널 포맷에 따라 섹션 이름이나 순서는 달라질 수 있지만, 보통 위 구성이 많이 활용됩니다.)

---

## 3. Technical Soundness를 높이는 핵심 요소

### 3.1 수학적 논리(Mathy Rigor)

1. **정의(Definitions)와 가정(Assumptions)**  
   - 강화학습(Reinforcement Learning)이라면 **MDP(Markov Decision Process)** 정의, 시계열 예측이라면 **확률 모델** 정의 등, 기본 개념부터 분명히  
   - “본 연구에서는 환경이 Markovian 속성을 가진다고 가정한다.” 처럼 가정을 명시

2. **수식 전개(Equations)**  
   - 알고리즘의 핵심이 되는 수식(예: 손실 함수, 업데이트 규칙, 확률적 추론) 을 구체적으로 제시  
   - “다음과 같은 손실 함수를 최소화한다.” “식 (2)는 (1)에서 출발해 라그랑주 승수를 적용했다.” 식의 **단계별 설명** 필요

3. **증명(Proof) or 스케치(Outline)**  
   - 완전한 증명이 길면 Supplementary(Material)에 넣고, 논문 본문에는 핵심 개념 혹은 Proof Sketch만 적을 수 있음  
   - 가능하면 “왜 이게 수렴하는지”, “왜 이게 최적 솔루션을 보장하는지”를 간략히라도 보여주면 **이론적 신뢰도**가 올라갑니다.

### 3.2 모델/알고리즘 설명(Implementation Details)

- **알고리즘 의사코드(pseudocode)**  
  - 한 페이지 이내 정도로, 단계별(입력, 반복 구조, 업데이트, 출력)로 정리하면 이해가 쉽습니다.  
  - 복잡한 최적화 알고리즘, Neural Network Layer 순서 등을 요약하기에 좋음

- **아키텍처 다이어그램**  
  - CNN, RNN, Transformer 등 신경망 구조가 핵심인 논문이라면, **블록 다이어그램**을 보여주면 한눈에 구조를 이해하기 용이  
  - 예: Encoder-Decoder, 멀티헤드 어텐션 모듈, Skip Connection 등

- **하이퍼파라미터/옵션**  
  - “학습률(learning rate)=1e-4, Optimizer=Adam, Beta1=0.9, Beta2=0.999, Batch Size=128 …”  
  - 본문에 모두 적기 너무 길면, 표 형태나 Supplementary로 넘겨도 됨  
  - 이 정보를 넣는 이유: **재현성**을 높이기 위함

### 3.3 복잡도/분석 (선택 사항이지만 권장)

- **시간 복잡도**: O(N^2), O(N log N) 등의 표기로 제안한 알고리즘이 기존 대비 얼마나 효율적인지 설명  
- **공간(메모리) 복잡도**: 대규모 AI 모델이라면 파라미터 수, GPU 메모리 사용량 등을 언급  
- **이론적 안정성/수렴성**: 예: “Proposition 1. Under Assumption A1~A3, the proposed algorithm converges to a local minimum in O(log t) time.” (간단한 증명 스케치)

---

## 4. 예시: 본론(Method) 문단 흐름

**2장. Proposed Method**  
**2.1 Overall Framework**  
- 그림 1 (Framework Overview): CNN Encoder + Attention Module + Classifier로 구성된 구조  
- 입력(X) -> Encoder (ResNet-50) -> Attention Layer -> Output(Y)  
- 잠재 표현을 학습할 때, Masked Reconstruction과정이 추가됨 (도식적으로 표현)  

**2.2 Objective Function & Training Scheme**  
- 식(1): L_total = L_classification + λ * L_reconstruction  
- L_classification은 Cross-Entropy Loss, L_reconstruction은 MSE 기반으로 정의  
- λ는 하이퍼파라미터로 0.1~0.5 범위를 실험  
- 학습 시, Adam Optimizer(β1=0.9, β2=0.999), learning rate 1e-4 적용  

(알고리즘 1: Pseudocode)  
```
Input: Training data D, batch size B
Initialize network parameters θ
for epoch in 1...E do
  for each mini-batch {x_i, y_i} in D do
      z_i = Encoder(x_i)
      x'_i = AttentionModule(z_i)
      loss = CE( Classifier(x'_i), y_i ) + λ * MSE(x'_i, x_i)
      θ = θ - η * ∇θ(loss)
  end
end
return θ
```
- 이런 식으로 알고리즘 단계를 한눈에 정리

**2.4 Complexity Analysis**  
- 시간 복잡도: O(N * d^2)로, 기존 Transformer 대비 20% 감소 (Attention 모듈이 축소형 구조)  
- 파라미터 수: 약 12M (ResNet-50에서 10M, Attention에서 2M)  
- 메모리 사용: 8GB GPU로 batch size=128 가능

(위 흐름은 예시이므로, 실제 논문 주제에 맞게 변형해 주세요.)

---

## 5. 작성 시 주의할 점

1. **독자가 따라갈 수 있는 순서**  
   - 큰 그림(Overview) → 세부 알고리즘(수식, 단계) → 구현/학습 세팅 → (가능하면) 이론 분석 …  
   - 순서가 뒤죽박죽이면 이해가 어렵고, 심사위원도 짜증(?!) 낼 수 있습니다.

2. **과도한 장황함 vs. 간결함**  
   - AI 모델 세부 구조가 복잡해도, 논문 지면(페이지)이나 독자의 집중력을 고려해 **핵심만 정리**하세요.  
   - 불필요한 반복 문장, 교과서적 일반 설명은 최소화(“CNN이란 무엇인가” 같은 내용은 Background 등에서 충분히 요약하거나, 인용으로 대체).

3. **그림/표/알고리즘** 활용**:**  
   - 글만 길게 써놓기보다는, **모듈 구조 그림**, **예시 입력/출력**, **의사코드** 등 **시각 자료**로 보완하면 이해가 훨씬 빨라집니다.

4. **참고문헌**(Reference) 철저히  
   - “이 부분은 (Kim et al., 2022)의 Sparse Attention 기법에서 차용했다” 처럼, 기존 아이디어를 인용해야 표절 이슈가 안 생깁니다.  
   - 표절, 중복 연구 시비를 피하기 위해 **원 출처**를 정확히 밝혀주세요.

---

## 6. 결론

**Method(본론) 파트**는 AI 논문의 **핵심 설계**를 담당합니다.  
- **기술적 타당성(Technical Soundness)**을 높이기 위해, **이론적 근거**(수식, 가정, 증명), **알고리즘 단계**, **실험 조건**을 구체적으로 쓰고,  
- **복잡도, 파라미터 수, 구현 디테일** 등을 꼼꼼히 밝히면, 학계와 산업계에서 **재현**과 **활용** 가능성을 높일 수 있습니다.

---

## 참고 자료

- *NeurIPS / ICML / ICLR 등 AI 컨퍼런스 Author Guidelines*  
- *Pytorch, TensorFlow Implementation Details* (공식 문서, GitHub)  
- *Goodfellow, I. et al. (2016). Deep Learning. MIT Press.*

---
