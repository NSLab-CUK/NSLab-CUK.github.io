---
layout: page
title: 부록(Appendix) 작성 방법
permalink: /lecture/material/intro-technical-writing/appendix
image: CUK_4Seasons.jpg
description: 부록이란, 본문에서 담기 어려운 추가 정보나 보조 자료를 따로 모아 정리하는 부분입니다.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

**부록**이란, 본문에서 담기 어려운 **추가 정보**나 **보조 자료**를 따로 모아 정리하는 부분입니다. AI 논문에서 부록은 다음과 같은 경우에 특히 유용합니다.

1. **장황하거나 세부적인 내용**:  
   - 본문에 모두 적으면 지면·분량이 지나치게 길어질 수 있는 내용 (예: 하이퍼파라미터 표, 추가 알고리즘 단계, 세부 증명 과정 등)  
2. **추가 실험·결과**:  
   - 본문에 싣기에는 너무 많은 그래프나, 간략히만 언급했던 추가 실험을 자세히 보여줄 때  
3. **데이터셋·코드 가이드**:  
   - 데이터셋 구성, 어노테이션 전략, 코드를 빌드·실행하는 방법 등.  
4. **이론적 증명(Proof)**:  
   - 간단한 요약은 본문에, 자세한 증명 절차는 부록으로 넘겨 깔끔하게 정리.

AI 논문에서는 투고 학회·학술지에 따라 “Supplementary Materials,” “Appendix,” “Extended Material” 등의 이름을 사용할 수 있으며, 대체로 별도의 PDF로 제출하는 경우가 많습니다.

---

## 1. 부록을 두는 이유

1. **본문 간결화**  
   - 주요 아이디어와 결과가 산만해지지 않도록, 반드시 필요한 내용만 본문에 담고, 세부적인 항목은 부록으로 옮겨서 전체 흐름을 깔끔하게 유지할 수 있습니다.

2. **추가 자료 제공**  
   - 연구 재현성(Replicability)을 높이기 위해, 실험 세팅·코드·데이터 스키마 등 자세한 정보를 제공해야 할 때가 많습니다.  
   - 분량 제한이 있는 학술지/학회라면, 이 정보는 부록으로 배치해도 충분히 좋습니다.

3. **이론 증명 보완**  
   - AI 논문에서 “왜 모델이 수렴하는가?”, “어떤 조건에서 최적 해를 보장하는가?” 같은 이론적 증명을 간단히만 본문에 요약하고, 상세 증명은 부록에 넣으면 편리합니다.

4. **추가 실험 또는 오류 사례 분석**  
   - Ablation Study나 에러 케이스 분석을 확장해서 보여주거나, 시각 자료가 많은 경우, 본문에 모두 배치하면 분량이 과도해집니다. 이럴 때 부록이 유용합니다.

---

## 2. 부록에 담을 수 있는 항목들

1. **알고리즘 상세 단계(Extended Pseudocode)**  
   - 본문에서는 핵심 알고리즘(의사코드)만 간략히 설명하고, 세부 반복 루프나 예외 케이스 처리는 부록에서 상세히 보여줄 수 있습니다.

2. **하이퍼파라미터 표**  
   - 모델마다 달라지는 **learning rate**, **batch size**, **optimizer 설정**, **dropout**, **regularization** 등 여러 파라미터를 표로 일괄 정리.  
   - 예:  
     | Model Variant  | Learning Rate | Batch Size | Optimizer | Dropout |
     |---------------|---------------|-----------|----------|---------|
     | Baseline      | 1e-3          | 64        | Adam     | 0.2     |
     | Proposed (A)  | 5e-4          | 128       | Adam     | 0.3     |
     | Proposed (B)  | 1e-4          | 128       | AdamW    | 0.3     |

3. **추가 실험 결과**  
   - 다른 데이터셋이나 다른 하이퍼파라미터 설정에서 나온 결과  
   - 비교 모델별 성능 표(Accuracy, F1, BLEU 등)를 추가로 제시  
   - 오류 사례 스크린샷(이미지 인식, 번역 결과, 생성 텍스트 등)

4. **데이터셋 세부 정보**  
   - 클래스 분포, 예시 이미지/문장, 어노테이션 방식, 라이선스나 윤리적 고려 사항 등  
   - 예: “본 데이터셋은 A/B 두 기관에서 수집하였으며, 환자 익명화 절차를 다음과 같이 진행하였다.”

5. **이론 증명(Proofs) 및 수학적 세부사항**  
   - 본문에서는 (Theorem, Lemma)를 간략하게만 언급한 뒤, 부록에 증명 과정을 단계별로 전개  
   - 예: “Lemma 1. [중략] 부록 A.1에서 증명함.”

6. **실험 코드 가이드**  
   - GitHub 링크, 실행 방법, 의존 라이브러리, 버전 정보 등을 구체적으로 기술(학술지·학회가 허용하면).  
   - 만약 깃 주소나 실행 지침을 본문에 넣기 불편하다면, 부록에 명시.

---

## 3. 부록 작성 시 주의사항

1. **본론-부록 연결**  
   - 본문에서 “세부 알고리즘은 부록 A에 제시하였음” 식으로 **명시적 연결**을 해주어야, 독자나 리뷰어가 쉽게 찾아볼 수 있습니다.  
   - Ex) “수학적 증명은 Appendix B에 상세히 기술하였다.”

2. **중복 서술 금지**  
   - 부록 내용이 본문과 중복되지 않도록 합니다.  
   - 본문에 이미 충분히 설명한 사항을 부록에 또다시 장황하게 적지 말고, 필요한 확장·보충 정보만 배치하세요.

3. **표기 방식 통일**  
   - 섹션 번호, 그림(표) 번호를 어떻게 부록에서 매기는지 **논문 전체**와 통일해야 합니다.  
   - 예: “Appendix A. Table A1, Fig. A1”처럼 별도 표기하거나, “Table 10, Figure 8”처럼 전반적 번호 연속성을 유지할 수도 있습니다. 규정에 맞춰 선택하세요.

4. **아카이브/저널 규정 확인**  
   - arXiv나 NeurIPS, ICML, ICLR 같은 AI 학회는 추가 PDF 첨부(“Supplementary Materials”)를 허용하되 **페이지 제한**이 있을 수 있습니다.  
   - 일부 학술지(IEEE/ACM)도 부록의 분량이나 첨부 형식을 제한하므로 **Author Guidelines**를 미리 확인하세요.

5. **민감 정보 주의**  
   - 만약 부록에 **개인정보**, **비식별이 충분하지 않은 데이터** 등이 들어가면 윤리적 이슈가 발생할 수 있습니다. 필요한 경우 가명처리, 마스킹, 승인 절차 등을 사전에 진행해야 합니다.

---

## 4. 예시 구조

아래는 AI 논문의 부록(Apendix) 예시 구조입니다.

Appendix A. Implementation Details
A.1 Hyperparameters
   - Table with learning rate, batch size, etc.
A.2 Model Variants
   - Explanation of “Proposed (A), Proposed (B)” differences

Appendix B. Additional Results
B.1 Extended Ablation Studies
   - Table B1: Performance under different dropout rates
B.2 Error Cases
   - Figure B1: Examples of misclassified images

Appendix C. Theoretical Proofs
C.1 Proof of Theorem 1
   - Detailed math steps
C.2 Proof of Lemma 3
   - Additional references

Appendix D. Dataset Information
D.1 Data Collection & Annotation
   - Ethical considerations
D.2 Class Distribution
   - Chart/diagram
D.3 Example Instances
   - Sample images or text snippets

Appendix E. Code & Environment Setup
E.1 GitHub Repository Link
E.2 Dependencies & Execution Commands

- 섹션 이름, 번호 체계는 **학회/저널 규정**에 맞춰 조정하시면 됩니다.  
- 본문에서 해당 부록을 “Appendix A” “Appendix B” 등으로 참조해 주면 **연결성**이 좋아집니다.

---

## 5. 작성 스타일 팁

1. **간결히, 명확히**  
   - 부록이라고 해서 **장황하게 쓰기보다는**, 독자가 필요한 정보를 **빠르게 확인**할 수 있도록 구성하세요.  
   - 표·그림을 잘 활용해 시각적으로 깔끔하게 전달하는 것도 좋습니다.

2. **부록 제목**  
   - “Appendix” 혹은 “Supplementary Materials”라고 크게 쓰고, 내부 섹션을 “A, B, C…” 등으로 나눠 관리합니다.  
   - “Appendix A. Detailed Pseudocode”처럼, 제목만 봐도 무슨 내용인지 알 수 있게.

3. **참고문헌 인용**  
   - 부록에서도 **인용**을 할 수 있으므로, 본문과 동일한 방식(번호 인용, 저자-연도 인용 등)을 따르세요.  
   - 별도의 ‘부록 참고문헌’을 두지 말고, 논문 전체의 참고문헌 목록과 통합되어야 합니다.

4. **그림/표 번호 매김**  
   - “Figure A1, Table B1” 등 부록용 번호를 따로 매길 수도 있고, “Figure 10, Table 12” 등으로 본문과 이어갈 수도 있습니다.  
   - 학회/저널마다 선호가 다르니, 가이드라인을 확인하세요.

---

## 6. 주의사항: 부록 분량과 내용 관리

- **과도한 분량**: 부록이 **본문보다 길어**지는 경우, 심사위원이 불편해하거나, 학회 규정 위반일 수 있음.  
- **무의미한 자료**: 의미 없이 중복된 그래프나, 별 효용이 없는 결과 표 등을 잔뜩 넣으면 오히려 독자에게 피로감을 줍니다.  
- **중요 내용을 본문에 넣어야 하는지 여부**: 만약 아주 핵심적인 실험 결과나 증명이라면 부록이 아니라 본문에 꼭 배치해야 합니다.

---

## 7. 결론

**부록(Appendix)**은 AI 논문에서 **가치 있는 부가 자료**를 담는 좋은 통로입니다.  
- 본문을 **간결**하게 유지하면서도, **연구 재현성**과 **추가 정보 제공**을 동시에 달성할 수 있죠.  
- 그러나 **분량**이나 **중복**, **학회 규정**에 유의해 **필요한 정보를 선택적으로** 배치해야 합니다.

---

## 참고자료

- *NeurIPS, ICML, ICLR, CVPR 등 AI 컨퍼런스 Author Kit*: Supplementary Material 관련 규정  
- *IEEE/ACM Transactions* 저널 가이드라인: Appendix, Online-Only Supplemental Files  
- *Overleaf Help Center*: “How to include Appendices in LaTeX”  
- *Goodfellow, Bengio, & Courville (2016). Deep Learning.* – 부록 참고 예시

---

