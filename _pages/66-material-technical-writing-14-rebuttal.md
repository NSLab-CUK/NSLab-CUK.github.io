---
layout: page
title: 컨퍼런스 Rebuttal 작성 방법
permalink: /lecture/material/intro-technical-writing/rebuttal
image: CUK_4Seasons.jpg
description: 이 글은 컨퍼런스에서 리뷰어 코멘트에 대한 재답변(Rebuttal) 과정과 Rebuttal(Author Response)를 작성하는 방법을 설명합니다.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

이 글은 **컨퍼런스에서 리뷰어 코멘트에 대한 재답변(Rebuttal)** 과정과 실제 **Rebuttal 문서(Author Response)**를 작성하는 방법을 설명합니다. 특히 **AI 분야** 대표 컨퍼런스(NeurIPS, ICLR, ICML 등)에서는 **1차 리뷰** 후, **짧은 기간** 내에 **저자가 리뷰어들의 의견에 응답**하는 과정을 갖습니다. 학술지(Journal)도 일부 상황에서 비슷한 “Revision & Response” 과정을 거치지만, **컨퍼런스**는 **짧은 기간**, **특정 형식(페이지·단어 제한)**, **더블 블라인드** 등 독특한 특징이 있으니 주의해야 합니다.

---

## 1. 컨퍼런스 Rebuttal(Author Response)란?

- **컨퍼런스 Rebuttal(Author Response)**:
  - 논문 투고 후, **리뷰어들(심사위원)**이 준 **피드백**을 저자가 **짧은 문서**로 답변하는 단계  
  - AI 분야 주요 컨퍼런스(NeurIPS, ICLR, ICML 등)에서는 리뷰 프로세스 중간에 **“Rebuttal 기간”**을 주어, 저자가 **명확한 반박 혹은 보충 설명**을 하도록 함  
  - 이 답변을 바탕으로 리뷰어들이 **최종 추천(accept/reject) 결정**에 대한 의견을 수정하거나 재확인할 수 있음

- **특징**:
  - **짧은 기간** (보통 3~7일 정도)  
  - **분량·형식 제한** (예: 1~2페이지 이내, 1,000~2,000단어 제한 등)  
  - **더블 블라인드** (저자 정보, 리뷰어 정보가 숨겨진 상태로 진행)  
  - 한정된 지면에서 **가장 중요**한 리뷰 포인트에만 집중해 답변해야 함

---

## 2. Rebuttal의 주요 목적

1. **오해나 사실관계 정정**  
   - 리뷰어가 논문을 오해하거나 잘못된 가정으로 비판했을 때, **정확한 맥락**을 전달해 **오류**를 바로잡는 것  
2. **추가 실험·근거 제시**  
   - 리뷰어가 요청한 **추가 결과**(예: 더 큰 데이터셋, 다른 베이스라인, Ablation)나 간단한 실험, 수치를 **가능한 범위 내**에서 제공  
3. **설명·clarification**  
   - “본 논문의 특정 부분이 불분명하다”는 코멘트에 대해 **문헌/근거**를 들어 더 자세한 설명  
4. **정중하고 설득력 있는 태도**  
   - 공격적·방어적 태도 대신 **협조적**으로, “리뷰어 피드백을 수용하고 논문을 개선하겠다”는 인상을 주어, **accept 가능성**을 높이는 역할

---

## 3. Rebuttal 작성 과정 & 전략

### 3.1 리뷰 코멘트 분석

1. **리뷰 요약**  
   - 각 리뷰어가 제기한 **핵심 포인트**를 정리(“Reviewer #1: ~, Reviewer #2: ~, Reviewer #3: ~”)  
   - 중복되는 이슈나 중요도가 큰 이슈를 **우선순위**로 배열  
2. **수용/설명/반박 분류**  
   - 어떤 코멘트는 **수정·보완**(수용) 가능,  
   - 어떤 코멘트는 **이미 논문에 있거나 오해**(설명 필요),  
   - 어떤 코멘트는 **본 연구 범위를 벗어남**(정중히 반박)  
3. **시간·자원 고려**  
   - 제한된 rebuttal 기간에 **새로운 실험**(컴퓨팅 자원, 데이터 재처리)이 가능할지 판단  
   - 불가능하면, “추후 카메라 레디에서 보완 가능” 등의 표현으로 대처

### 3.2 문서 구조(일반적인 형식)

- **인사 & 감사를 짧게 (선택)**  
  - 예: “We thank all reviewers for the constructive feedback…”  
- **전반적 요약** (리뷰 공통이슈에 대한 전체 답변)  
  - “Several reviewers requested additional comparisons. We provide them in Table A below…”  
- **리뷰어별 상세 답변**  
  - “**Reviewer #1**: Q1) ~~, Q2) ~~, A1) …, A2) …” 식으로 구조화  
  - 댓글(코멘트) 인용 → 저자의 답변 형식  
- **결론/마무리 (선택)**  
  - “We appreciate the reviewers’ time and will incorporate these clarifications in the final version.”

### 3.3 글쓰기 방법 & 톤

1. **정중한 어조**  
   - 긍정적 표현: “We appreciate the suggestion…”, “This is an excellent point…”  
   - 비판적 지적이라도 “We understand the concern…”으로 시작해, 성급한 반박 tone을 피함  
2. **간결한 문장**  
   - Rebuttal 분량이 매우 제한적이므로, 불필요한 서술은 자제  
   - “As requested, we ran an additional experiment on XYZ dataset. The results are in Table 1 below.”  
3. **테이블·도표·숫자 활용**  
   - 짧은 답변이라 해도, **새로운 결과**는 간단한 테이블/그림으로 **명확히** 보여주면 **설득력**이 커짐  
4. **구체적 근거 제시**  
   - “We achieve 88.5% (±0.2) on the new baseline, surpassing X et al. (2021) by +1.2%. The training details are in the supplementary.”  
5. **요청 사항에 대한 정확한 대응**  
   - 리뷰어가 “다른 베이스라인과 비교”를 요구했으면, **어느 베이스라인**을, **어떤 세팅**으로, **결과가 어떠했는지**를 간단히 보여줘야 함  
   - 불가능하면, “Due to time constraints, we cannot complete a thorough test. However, we plan to include it in the final version if the paper is accepted.”

---

## 4. 자주 마주치는 상황별 작성 팁

1. **오해나 오류 지적**  
   - “Reviewer #2 states that we use dataset ABC, but actually, we used dataset XYZ. We apologize for any confusion. We clarified this in Sec. 3.2 of the updated version.”  
   - 차분히 **사실 관계**를 재확인하고, 문서상 **어디에서** 잘 드러나지 않았는지 언급

2. **추가 실험 요청**  
   - “We ran the requested ablation on the synthetic dataset with the same hyperparameters. As shown in Table 2, our method still improves by +1.5%.”  
   - 컴퓨팅 리소스가 있어 **간단한 실험 가능**하면 해주되, **시간이 부족**하면 “We will add this in the final version due to limited time in the rebuttal period.”

3. **관련 문헌 부족**  
   - “We appreciate pointing out the relevant works by [Smith et al., 2020]. We have reviewed them and will cite/discuss them in Sec. 2.2. They indeed share a similar motivation but approach the problem differently…”  
   - 필요하면 짧게 차이점 언급

4. **과도한 확장 요청**  
   - 예: “We request the authors to test on 10 additional datasets.” → 시간적·자원적 한계로 곤란  
   - 정중히: “Due to the limited scope and timeframe, a full expansion to 10 new datasets is not feasible at this moment. However, we are happy to incorporate at least 1–2 more for the final version if accepted.”  

5. **리뷰어 점수/결정과 무관한 질문**  
   - 어떤 리뷰어는 **호기심**으로 질문할 수도 있음(“Could this method also apply to medical imaging?”).  
   - 최대한 **요령껏** 답하되, 논문 범위를 벗어난다면 그 사실을 부드럽게 명시(“This is beyond our current focus, but we see potential for future exploration.”).

---

## 5. 간략한 Rebuttal 템플릿

**We thank the reviewers for their time and valuable comments. Below, we address each concern.**

-------------------
1. Common Concerns
-------------------
- Comparison with Additional Baselines
  We include new results with [ABC model, CVPR'21] in Table 1. Our method outperforms ABC by +0.8% in accuracy on the X dataset. 
- Clarity on Dataset Split
  Some reviewers noted confusion about train/val splitting. We clarify that we followed the standard protocol from [Z et al., 2019].
  
----------------------
2. Reviewer #1 Comments
----------------------
(1) "The approach might rely too heavily on labeled data..."

  **Response**: 
  - We appreciate this concern. Actually, our method is semi-supervised, using ~40% labeled data and 60% unlabeled data. 
  - We added clarifications in Sec. 3.2, referencing Appendix A for a more detailed pipeline.

(2) "Experiment on dataset B would strengthen the claim."

  **Response**:
  - We ran a quick test on dataset B. Table 2 shows +1.5% gain over baseline, confirming our approach generalizes. 
  - Details on training settings are in the supplementary.

----------------------
3. Reviewer #2 Comments
----------------------
(1) "Cite Smith et al. (2020)."

  **Response**:
  - Thank you for pointing this out. We have now cited Smith et al. (2020) in Sec. 2 and discussed similarities/differences.

(2) "Include multi-GPU scaling results."

  **Response**:
  - Due to limited time, we cannot present full multi-GPU scaling tests. However, preliminary results in Appendix B indicate near-linear speedup. We plan to expand this in the final version.

-----------------------------------
4. Reviewer #3 Comments (Minor Points)
-----------------------------------
- We corrected a notation error in Eq. (4). 
- Figure 3 is updated with a higher-resolution version.

In summary, we appreciate the constructive feedback and believe these clarifications and additional data strengthen our work. We hope our responses address the reviewers’ concerns adequately, and we look forward to improving the paper further.

Sincerely,
(The Authors)

---

## 6. 제출 후 & 마무리

- Rebuttal 제출 후, **리뷰어**는 이를 확인하고, 자신의 점수(accept/reject)에 대한 의견을 다시 조정할 수 있습니다.  
- 결과 발표까지 추가 질문이 오지는 않으나, 컨퍼런스와 **에디터**/**AC(Area Chair)**가 원하는 경우 **추가 정보**를 요청할 수 있으니, **항상 준비**해두세요.  
- 최종적으로 **accept** 시, **카메라 레디**(camera-ready) 버전에 **Rebuttal에서 약속한 수정 사항**을 반영하면 됩니다.

---

## 7. 결론

- **컨퍼런스 Rebuttal**은 **짧은 시간**, **제한된 분량** 안에서 **필요한 정보를 최대한** 제공하여,  
  - **리뷰어의 오해를 풀고**,  
  - **추가 요청**(실험·분석)에 응하거나 불가능한 사유를 정중히 설명하며,  
  - **논문의 가치**를 **재강조**하는 역할을 합니다.

- **핵심**:
  - 1) 리뷰어가 궁금해 하는 점 **정확히** 파악,  
  - 2) **정중·간결·구체적**인 답변,  
  - 3) 가능하다면 **간단한 추가 실험 결과**를 제시해 **신뢰도**를 높인다.  

---

## 참고 자료

- **NeurIPS / ICLR / ICML Author Instructions**: 공식 웹사이트에 종종 Rebuttal(Author Response) 가이드가 있음  
- **OpenReview**(ICLR 플랫폼)에서 다른 논문들의 Rebuttal 사례 확인 가능  
- 학술 커뮤니티(예: Reddit r/MachineLearning, Twitter)에 공유된 Rebuttal Tips, 에디터·AC 인터뷰  
- **“How to respond to reviewers’ comments”** (Enago, Editage 등 학술에디팅 블로그)

---

