---
layout: page
title: 학술문헌 서지정보 정리 방법 & BibTeX 활용법 II
permalink: /lecture/material/intro-technical-writing/bibtex-2
image: CUK_4Seasons.jpg
description: 이 글에서는 LaTeX + BibTeX + JabRef + Overleaf 조합을 활용할 때, “학술문헌 종류별 서지정보 정리 방법”과 **“BibTeX 필드별 상세 가이드”**를 세부적으로 안내합니다.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

이 글에서는 LaTeX + BibTeX + JabRef + Overleaf 조합을 활용할 때, **“학술문헌 종류별 서지정보 정리 방법”**과 **“BibTeX 필드별 상세 작성 가이드”**를 세부적으로 안내합니다.

---

# 학술문헌 서지정보 정리 방법 & BibTeX 활용법  
### (LaTeX + JabRef + Overleaf, 문헌 종류별 & 필드별 상세 가이드)

연구, 논문, 레포트, 프로젝트 보고서를 쓰다 보면 **참고문헌**이 점점 늘어납니다.  
한두 편은 수기로 적어도 되지만, 10편, 20편 넘어가면 **항상 같은 문제**가 생깁니다.

- “아, 이거 저널명이 뭐였지?”  
- “저자명을 원어 그대로 적어야 하나, 로마자로 바꿔야 하나?”  
- “표기 형식(APA, IEEE, Chicago 등)이 바뀌는데, 한두 줄 수정으로 끝났으면 좋겠는데…”

이 글에서는 **LaTeX + Overleaf** 환경에서 **JabRef**로 서지정보를 **체계적**으로 관리하고, **BibTeX**로 자동 인용·참고문헌 생성을 완성도 높게 하는 방법을 안내합니다. 특히 **학술문헌 종류별**(학술지 논문, 학회 발표논문, 도서, 보고서, 웹자료 등)로 **어떤 필드를 어떻게 기입하면 좋을지**까지 자세히 살펴보겠습니다.

---

## 1. 다양한 학술문헌 유형과 BibTeX 타입

BibTeX에는 여러 **문헌 타입**(Entry Types)이 존재합니다. 대표적으로 다음과 같은 것들이 있습니다.

| BibTeX 타입     | 주로 사용되는 문헌 종류                          | 예시                                              |
|----------------|-----------------------------------------------|--------------------------------------------------|
| `@article`     | 학술지(저널) 논문                               | Nature, IEEE Transactions, 각종 학회지 논문 등     |
| `@inproceedings` (또는 `@conference`) | 학회(컨퍼런스) 발표 논문                        | SIGKDD, ACL, CVPR, CHI 등 국제학회 발표 논문       |
| `@book`        | 단행본(저서)                                    | 전공 교재, 연구서, 일반 서적 등                   |
| `@inbook`      | 책의 특정 장(Chapter)                          | 편저서 내 특정 챕터, 편집된 도서에 실린 글 등       |
| `@techreport`  | 기술보고서, 연구보고서                           | 정부/기관/연구소 보고서, 프로젝트 최종보고서 등    |
| `@misc`        | 기타(웹사이트, 신문기사, 온라인 자료 등)          | 블로그, 웹문서, 강의노트, Github README 등          |
| `@mastersthesis`, `@phdthesis` | 학위 논문(석사/박사)                      | 석사 학위논문, 박사 학위논문                       |

아래에서는 **학술논문(저널/학회), 도서, 보고서, 웹자료** 4가지 유형을 중심으로, **어떤 BibTeX 필드들을 주로 채워야 하는지**를 예시와 함께 제시해 드리겠습니다.

---

## 2. BibTeX 필드별 상세 설명

BibTeX는 각 타입에 맞게 필드를 **필요(Required), 권장(Optional), 확장(Additional)** 세 가지로 나눕니다.  
아래 표는 대표적인 필드들의 역할과 작성 팁을 요약한 것입니다.

| 필드명       | 설명                                                      | 작성 팁                                                                    |
|-------------|----------------------------------------------------------|----------------------------------------------------------------------------|
| `author`    | 저자(들) 이름                                            | 복수 저자일 때는 “and”로 구분 (예: `author = {Hong, Gil-dong and Kim, Min-jun}`)|
| `editor`    | 편집자                                                   | @inbook, @proceedings, @book 등에서 편집자 정보가 필요할 때 사용            |
| `title`     | 논문/도서/챕터/보고서 제목                                | LaTeX 특수문자(&, %, # 등)는 `\&`, `\%`, `\#` 식으로 이스케이프             |
| `journal`   | 학술지(저널) 이름(@article)                              | 예: `journal = {IEEE Transactions on Computers}`                          |
| `booktitle` | 학회(컨퍼런스) 명(@inproceedings)                        | 예: `booktitle = {Proceedings of the 40th ICML}`                           |
| `year`      | 발행 연도                                                | 숫자만 적되, 필요하면 `month` 필드에 월 정보 별도 기재                     |
| `volume`    | 권(Vol.)                                                 | 저널/책 등 발행물의 권수                                                   |
| `number`    | 호(No.)                                                  | 권(Volume) 내 세부 호수                                                   |
| `pages`     | 페이지 범위                                              | 예: `345--360` (하이픈은 `--`로)                                          |
| `publisher` | 출판사/발행기관                                          | 도서(@book), 보고서(@techreport) 등에서 자주 사용                         |
| `institution` | 기관 이름(@techreport)                                 | 예: `institution = {한국과학기술연구원(KIST)}`                             |
| `organization`| 학회/학술대회 주관 단체명(@inproceedings)              | 예: `organization = {ACM}`                                                |
| `school`    | 학교 이름(@mastersthesis, @phdthesis)                   | 예: `school = {Seoul National University}`                                |
| `doi`       | DOI(Digital Object Identifier)                          | 예: `doi = {10.1109/TKDE.2019.1234567}`                                  |
| `url`       | 웹 링크                                                 | @misc 또는 온라인 자료를 명시할 때                                           |
| `howpublished` | 발행/배포 형태(@misc)                                 | 예: `howpublished = {\url{https://example.com/report}}`                  |
| `note`      | 기타 부가 정보                                           | 부록, 수정판, 번역판 등에 대한 간단한 설명                                |

각 타입마다 필드 요구사항이 다르므로, JabRef나 다른 BibTeX 문서를 참고하면 됩니다.  
하지만 여기서는 실무적으로 **“어떤 정보를 최소한으로 기입하면 좋을지”**에 초점을 맞추어 설명하겠습니다.

---

## 3. 문헌 종류별 예시 & 필드 구성

### 3.1 저널 논문 (`@article`)

- **필수 필드**: `author`, `title`, `journal`, `year`  
- **권장 필드**: `volume`, `number`, `pages`, `doi`  
- **추가 필드**: `month`, `publisher`(드물게), `url` 등

```bibtex
@article{lee2022nlp,
  author    = {Lee, Sunghoon and Kim, Jihyun},
  title     = {A Comparative Study of Transformer Models for NLP},
  journal   = {Journal of Language AI},
  volume    = {12},
  number    = {4},
  pages     = {345--360},
  year      = {2022},
  doi       = {10.1000/jlai.2022.045}
}
```

**작성 팁**  
- 저자(Author) 여러 명일 때 **“and”**로 구분합니다. (`Lee, Sunghoon and Kim, Jihyun`)  
- `title` 필드에서 “&” → `\&` 로, “%” → `\%` 로 **이스케이프**.  
- 가능하면 `doi`를 꼭 입력해두면, BibTeX 출력 시 DOI 링크를 자동 생성해줄 수도 있습니다(스타일에 따라).

---

### 3.2 학회(컨퍼런스) 발표 논문 (`@inproceedings` 또는 `@conference`)

- **필수 필드**: `author`, `title`, `booktitle`, `year`  
- **권장 필드**: `pages`, `organization`, `publisher`, `doi`  
- **추가 필드**: `volume`(워크숍/특별 세션일 때), `editor`(프로시딩 편집자), `url`

```bibtex
@inproceedings{park2023chatgpt,
  author    = {Park, Areum and Choi, Gihyun},
  title     = {Exploring Large Language Models in ChatGPT for Education},
  booktitle = {Proceedings of the 56th ACM Technical Symposium on Education},
  year      = {2023},
  pages     = {101--110},
  organization = {ACM},
  doi       = {10.1145/1234567.1234569}
}
```

**작성 팁**  
- `booktitle`은 **학술대회(프로시딩) 이름**을 정확히 기입하세요(“Proceedings of…”로 시작하는 경우 많음).  
- 대규모 학회(예: ACM, IEEE 등)일 경우 `organization`에 주최 단체 이름을 적습니다.

---

### 3.3 도서(단행본) (`@book`)

- **필수 필드**: `author`(또는 `editor`), `title`, `publisher`, `year`  
- **권장 필드**: `edition`, `volume`(시리즈 물일 경우), `isbn`, `doi`  
- **추가 필드**: `series`, `address`(출판 도시, 구형 BibTeX에선 사용), `url`

```bibtex
@book{smith2021deep,
  author    = {Smith, John and Brown, Emily},
  title     = {Deep Learning in Practice},
  publisher = {Springer},
  year      = {2021},
  edition   = {2nd},
  isbn      = {978-3-030-12345-6}
}
```

**작성 팁**  
- 저자가 여러 명인 경우 `author`에 모두 나열. 편집 도서라면 `editor` 필드를 사용합니다.  
- `edition`에 **“1st”, “2nd”**와 같은 정보를 넣어주면, 참고문헌 표기 시 도움이 됩니다(스타일에 따라 자동 표기).

---

### 3.4 연구보고서 / 기술보고서 (`@techreport`)

- **필수 필드**: `author`, `title`, `institution`, `year`  
- **권장 필드**: `number`(보고서 번호), `month`, `url`  
- **추가 필드**: `type`(“Research Report”, “Technical Report” 등 구체 명시)

```bibtex
@techreport{kang2020kisti,
  author      = {Kang, Heesoo},
  title       = {AI Adoption in Healthcare: A Technical Survey},
  institution = {KISTI (Korea Institute of Science and Technology Information)},
  year        = {2020},
  number      = {TR-2020-45},
  type        = {Technical Report},
  url         = {https://example.org/kisti-report.pdf}
}
```

**작성 팁**  
- 정부 부처, 연구소, 기업 등 **발행기관**을 `institution` 필드에 정확히 적습니다.  
- 보고서 고유 번호가 있다면 `number` 필드에 기재.  
- 웹에서 다운로드 가능한 공개 자료라면 `url` 필드도 활용하세요.

---

### 3.5 웹자료 / 기타 (`@misc`)

- **필수 필드**: (규정 없음, 상황에 맞춰 `author`, `title`, `howpublished`, `year` 등을 활용)  
- **권장 필드**: `url`, `note`, `author`(있다면), `month`  
- **추가 필드**: `lastchecked`(날짜), `urldate`(접속일)

```bibtex
@misc{jones2023blog,
  author       = {Jones, Michael},
  title        = {Understanding GPT-4: A Layman's Guide},
  howpublished = {\url{https://medium.com/@mikejones/gpt4-guide}},
  note         = {Accessed: 2023-07-10},
  year         = {2023}
}
```

**작성 팁**  
- 웹페이지, 블로그, 온라인 매뉴얼, 위키문서 등은 형태가 매우 다양하므로, 가능한 정보를 최대한 기재합니다.  
- `howpublished`에 `\url{…}` 문법을 쓰면, LaTeX에서 클릭 가능한 링크로 출력되는 경우가 많습니다.  
- 접속일을 기재해야 하는 스타일(예: APA 7th)이라면 `urldate` 필드를 쓰거나 `note`에 “Accessed:” 형식으로 적어둡니다.

---

## 4. JabRef에서 문헌 타입과 필드 관리하기

### 4.1 문헌 타입 자동 인식

- JabRef에 BibTeX를 드래그&드롭하면, 자동으로 문헌 타입(@article, @inproceedings 등)을 감지합니다.  
- 정확하지 않은 경우, JabRef 우측 패널에서 **“Change entry type”** 버튼을 눌러 수정할 수 있습니다.

### 4.2 필드별 입력 가이드

- JabRef 우측 패널에 **Required/Optional/General/Review** 탭이 표시됩니다.  
- “Required fields” 아래에 빨간색 느낌표가 있으면, **BibTeX 표준상 필수 필드가 비어있다**는 뜻이니 확인해 주세요.  
- “Optional fields”에도 `doi`, `url`, `abstract` 등 추가 정보를 넣으면, 나중에 검색과 관리가 훨씬 편해집니다.

### 4.3 사용자 정의 필드

- 필요한 경우, JabRef “Options > Customize entry types” 메뉴에서 **필드를 추가**하거나 **순서를 바꿀 수** 있습니다.  
- 예: 특정 연구기관 보고서는 `projectid` 같은 고유 키를 사용한다면, 사용자 정의 필드로 추가해둘 수 있음.

---

## 5. Overleaf에서 BibTeX 필드 사용 확인

LaTeX 문서에서 다음과 같은 스타일(.bst 파일 또는 biblatex) 설정에 따라 **출력 양상**이 달라집니다.

- `\bibliographystyle{plain}`: 기본 스타일, 저자명(이니셜), 연도, 제목, 저널 순  
- `\bibliographystyle{IEEEtran}`: IEEE 형식, [숫자] 인용, 저자명 이니셜, 제목 소문자  
- `\bibliographystyle{apalike}` 혹은 `\bibliographystyle{apacite}`: APA식, 저자(연도), 제목, DOI 등  
- BibLaTeX + `\usepackage[style=apa]{biblatex}`: APA 7th 방식 등 훨씬 유연한 설정 가능

필드를 충실히 입력했더라도, 스타일 파일이 해당 필드를 **출력 안 하는 경우**도 있습니다.  
예를 들어, `url`이나 `doi` 필드를 아예 무시하는 스타일이 존재할 수 있죠.  
그래서 **투고할 저널의 요구 사항**(어떤 스타일을 쓰는지, DOI나 URL을 넣어야 하는지)을 미리 파악하고,  
필요한 필드는 꼼꼼히 채우는 것이 좋습니다.

---

## 6. 자주 겪는 문제 & 해결책

1. **특수문자 에러**:  
   - 제목에 “%”나 “&”가 들어가면 LaTeX 컴파일 에러 발생 → 반드시 `\%`, `\&` 등으로 치환.  
2. **한글 깨짐**:  
   - JabRef에서 저장한 .bib 파일이 ANSI 인코딩이면, Overleaf(UTF-8)와 충돌 발생 → JabRef 설정에서 Encoding을 **UTF-8**로 통일.  
3. **BibTeX 키 중복**:  
   - `kim2023`이라는 키가 두 레퍼런스에 동시에 부여 → Overleaf 컴파일 시 Warning → JabRef에서 하나를 `kim2023a`로 변경 필요.  
4. **웹자료 날짜 표기**:  
   - @misc로 된 웹자료가 표준 스타일에서 적절히 표시되지 않을 수 있음 → BibLaTeX의 `urldate` 필드를 쓰거나, `note` 필드에 “Accessed: yyyy-mm-dd” 명시.  
5. **인용 순서가 안 맞음**:  
   - IEEE 스타일은 첫 인용이 [1], 두 번째가 [2]… 로 되어야 하는데, LaTeX가 재컴파일 전까지 레퍼런스 번호를 제대로 정렬 못 할 수 있음 → **두 번 이상** 빌드 필요.

---

## 7. 마무리: 철저한 필드 입력이 곧 완성도의 열쇠

다양한 문헌 유형을 다루다 보면, **어떤 정보가 꼭 필요하고, 어떤 건 선택 사항인지** 헷갈릴 수 있습니다.  
하지만 **JabRef**가 있으면, 필수 필드를 깜빡하지 않도록 도와주고, **LaTeX + Overleaf** 환경에서 **BibTeX**로 인용까지 매끄럽게 연결할 수 있습니다.

1. **문헌 종류별(저널, 학회, 도서, 보고서, 웹) 필드**를 숙지하면, 누락 없이 입력 가능  
2. **키워드, 태그, 메모** 등을 챙겨두면, 나중에 스스로 검색하거나 후속 연구에 재활용하기 편함  
3. **학술지 투고 규정**(인용 스타일, DOI/URL 표기 여부)을 먼저 확인하면, 중간에 포맷을 바꾸느라 고생할 일 줄어듦  
4. **LaTeX & Overleaf**에서 스타일 파일(bst) 또는 BibLaTeX 옵션에 따라 출력 결과가 달라질 수 있으니 주의  

---

## 참고 링크

- [JabRef 공식 문서](https://docs.jabref.org/) – 문헌 타입별 필드 설명, 고급 기능 안내  
- [BibTeX Entry Types (official)](http://www.bibtex.org/Usage/) – 전통 BibTeX 기본 사항  
- [BibLaTeX 패키지 문서](https://ctan.org/pkg/biblatex) – 확장 필드와 고급 스타일 설정 가이드  
- [Overleaf + BibTeX Tutorials](https://www.overleaf.com/learn/latex/Bibliography_management_with_bibtex)  

---

