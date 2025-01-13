---
layout: page
title: Reference (참고문헌) 작성 방법
permalink: /lecture/material/intro-technical-writing/reference
image: CUK_4Seasons.jpg
description: 논문을 작성할 때, 레퍼런스(참고문헌)는 단순히 ‘논문 뒤에 붙이는 리스트’ 이상입니다. 인용 스타일을 올바르게 사용하는 것은 연구 윤리와 학술적 신뢰도를 지키는 첫걸음이며, 정확한 서지정보는 후속 연구자(혹은 심사위원)가 관련 선행 연구를 쉽게 추적할 수 있도록 돕습니다.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

논문을 작성할 때, **Reference(참고문헌)**는 단순히 ‘논문 뒤에 붙이는 리스트’ 이상입니다.  
- **인용 스타일**을 올바르게 사용하는 것은 **연구 윤리**와 **학술적 신뢰도**를 지키는 첫걸음이며,  
- **정확한 서지정보**는 후속 연구자(혹은 심사위원)가 **관련 선행 연구**를 쉽게 추적할 수 있도록 돕습니다.

---

## 1. 왜 AI 논문에서 Reference가 더욱 중요한가?

1. **빠른 기술 변화와 다수의 자료**  
   - AI 분야는 폭발적으로 논문이 쏟아집니다(arXiv, NeurIPS, ICML, CVPR 등).  
   - 다양한 연구를 참조하며 최신 흐름을 반영할 수 있지만, 그만큼 **인용 관리**가 복잡해질 수 있습니다.

2. **연구 윤리와 표절 방지**  
   - 모델 구조나 알고리즘 아이디어를 본인이 새롭게 제안한 것처럼 ‘표절’하지 않도록, 원 출처(논문, 코드 레포지토리 등)를 **정확히 기재**해야 합니다.

3. **재현 가능성(Replicability)**  
   - 어떤 데이터셋, 어떤 알고리즘에서 영감을 받았는지 정확히 남겨두면, 후속 연구자가 **비교 실험**이나 **재현**을 하기 쉬워집니다.

4. **학술지/학회 요구사항**  
   - NeurIPS, ICML, ICLR 등 국제 학회는 **양식(스타일)**을 엄격히 요구합니다. APA, IEEE, ACM, Chicago 등 다양한 인용 스타일에 맞춰야 할 때도 있습니다.

---

## 2. 대표적인 Reference 스타일

1. **IEEE 스타일**  
   - 엔지니어링·컴퓨터공학 분야에서 흔히 사용. **숫자**([1], [2]) 기반 인용.  
   - 예)  
     > \[1\] Y. LeCun, Y. Bengio, and G. Hinton, “Deep learning,” *Nature*, vol. 521, pp. 436–444, 2015.

2. **APA 스타일 (7th ed.)**  
   - 사회과학·심리학 분야에서 주로 쓰이지만, **딥러닝+교육**, **인간-AI 상호작용(HCI)** 연구에서도 종종 사용. **(저자, 연도)** 기반 인용.  
   - 예)  
     > LeCun, Y., Bengio, Y., & Hinton, G. (2015). Deep learning. *Nature, 521*, 436–444.  

3. **ACM 스타일**  
   - 컴퓨터 과학 학회인 ACM의 저널·컨퍼런스에서 자주 사용.  
   - 예)  
     > [1] Y. LeCun, Y. Bengio, and G. Hinton. 2015. Deep learning. *Nature* 521 (2015), 436–444.

*(학회·저널에 따라 요구하는 스타일이 다르니, 투고하기 전 **Author Guidelines**를 반드시 확인하세요.)*

---

## 3. Reference 작성 시 체크리스트

1. **저자명, 제목, 학회/저널명, 연도, 페이지** 등 서지정보가 **정확**한가?  
2. **arXiv** 논문 인용 시, arXiv ID(예: arXiv:2107.0001), 업로드 연도, 버전 등을 명시했는가?  
3. **DOI**, **URL**(가능하다면)로 독자가 문서를 쉽게 찾을 수 있게 했는가?  
4. **GitHub** 등 코드 레포지토리 인용 시, **저자(소유자) + 저장소명 + commit/tag** 등을 기재했는가?  
5. **데이터셋**(예: ImageNet, COCO, GLUE)처럼 유명한 자료도, 해당 논문/논문집을 찾아 출처를 남겼는가?

---

## 4. 구체적인 작성 팁 & 예시

### 4.1 arXiv 논문 인용 방법

- arXiv는 정식 출판이 아니므로, 학회에 따라 ‘Preprint’로 취급될 수 있음.  
- 예) IEEE 스타일에서 arXiv 인용  
  ```
  [1] T. Brown, B. Mann, N. Ryder, et al., “Language Models are Few-Shot Learners,” 
      arXiv:2005.14165, 2020.
  ```
- 가능하면 “arXiv:XXXX.XXXXX [cs.LG], version X, 2020”처럼 **분야**와 **버전**도 기재가 좋음.

### 4.2 GitHub 레포지토리 인용

- 예)  
  ```
  @misc{paszke2019pytorch,
    author = {Paszke, Adam and Gross, Sam and Massa, Francisco and others},
    title  = {PyTorch: An Imperative Style, High-Performance Deep Learning Library},
    howpublished = {\url{https://github.com/pytorch/pytorch}},
    year   = {2019}
  }
  ```
- “commit id”나 “release tag”를 적으면 버전 관리에 도움이 됨.  
- 일부 학회는 소스 레퍼지토리에 대한 인용을 제한하거나, 논문 형태로만 인용하길 요구하기도 하니 규정 확인 필요.

### 4.3 데이터셋 인용

- 유명한 **ImageNet**의 경우, “ImageNet: A Large-Scale Hierarchical Image Database (CVPR 2009)” 논문을 참고문헌에 넣어야 함.  
- **COCO**는 “Microsoft COCO: Common Objects in Context (ECCV 2014)”.  
- 보통 데이터셋 이름과 함께 **원 논문** 혹은 **공식 사이트**를 인용하면, 독자들이 쉽게 찾아볼 수 있음.

### 4.4 표절과 자가표절 방지

- **본인이 예전에 쓴 논문**에서 일부 문장/아이디어를 가져올 때도, 꼭 해당 논문을 인용하는 것이 원칙(자가표절 방지).  
- **ChatGPT 등 LLM**에서 얻은 아이디어나 텍스트를 그대로 사용하면, 출처를 제시할 방법이 모호해지고 표절 이슈가 생길 수 있음. 따라서 **스스로 재검토**가 필수.

### 4.5 주의해야 할 함정

- **오탈자**: 저자명 철자, 논문 제목에서 “&, #, ~, :” 등 특수문자 누락 or 잘못 이스케이프  
- **연도 불일치**: 본문에서 (Kim et al., 2021)라고 써놓고 레퍼런스에 2020으로 기재  
- **페이지 번호**나 **권(Volume)** 누락  
- **Proceedings**(학회명, 장소, 날짜) 누락

---

## 5. 작성 시 주의사항

1. **본 문장과 Reference 매칭**  
   - 본문에 “(Krizhevsky et al., 2012)” 혹은 “[1]”라고 썼으면, 반드시 레퍼런스 리스트에도 해당 항목이 있어야 합니다(숫자·연도 일치).  
2. **일관성**  
   - IEEE 스타일이면 전부 IEEE 스타일, APA면 전부 APA. **혼합 사용 금지**.  
3. **최신 버전**  
   - arXiv나 GitHub 레포가 버전 업데이트될 수 있으므로, **논문 작성 시점** 기준으로 확인합니다.  
4. **표절 방지**  
   - 레퍼런스를 언급했더라도, 본문 문장을 **과도하게 복사**해 오면 표절이 될 수 있으니, **인용 형태(직접 인용 vs. 간접 인용)**에 유의해야 합니다.

---

## 6. 결론

**레퍼런스(참고문헌)**는 연구 윤리와 논문의 신뢰도를 지탱하는 **기초이자 마무리**입니다.  
- AI 논문은 인용할 자료가 매우 다양(arXiv, GitHub, 주요 학회 Proceedings, 데이터셋 등)하므로, **형식**과 **정확성**에 더욱 신경 써야 합니다.  
- BibTeX·Zotero·Mendeley 등 **관리 툴**을 적극 활용하면, **인용 양식**을 자동 변환하고 **오탈자**를 줄일 수 있습니다.

---

## 참고자료

- *IEEE Citation Reference* (IEEE 공식 문서)  
- *BibTeX.org (Official Usage & FAQ)*  
- *M. E. J. Newman, “How to Cite References,” *Physics Today*, vol. 62, no. 5, pp. 1–2, 2009.*  
- *Zotero / Mendeley / EndNote 사용자 가이드*  

---

