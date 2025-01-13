---
layout: page
title: 학술문헌 서지정보 정리 방법 & BibTeX 활용법 I
permalink: /lecture/material/intro-technical-writing/bibtex-1
image: CUK_4Seasons.jpg
description: 이 글에서는 LaTeX + BibTeX + JabRef + Overleaf 조합을 활용해, 서지정보를 깔끔하게 정리하는 방법을 상세한 단계별로 설명합니다.
toc: true
toc_sticky: true
toc_label: "Table of Contents"
---

논문이나 레포트를 작성할 때, **서지정보(References) 관리**는 매우 중요한 일 중 하나입니다. 인용과 참고문헌을 제대로 정리하지 않으면 표절 문제부터 학술적 신뢰도 하락까지 다양한 문제가 생길 수 있기 때문이죠. 특히 **LaTeX**를 통해 논문/보고서를 작성하고, 이를 **Overleaf**에서 협업하며, **JabRef**로 레퍼런스를 관리하면 — “인용 스타일 변경, 공동 작업, 참고문헌 자동화”가 모두 손쉬워집니다.

이 글에서는 **LaTeX + BibTeX + JabRef + Overleaf** 조합을 활용해, 서지정보를 깔끔하게 정리하는 방법을 **상세한 단계**별로 안내합니다.

---

## 1. 왜 LaTeX + JabRef + Overleaf인가?

1. **LaTeX**  
   - 학술 논문 및 기술 문서를 작성할 때, 서식·수식·참고문헌 처리를 자동화하여 **고품질** 문서를 손쉽게 만들 수 있는 툴입니다.  
   - `.tex` 파일로 문서를 작성하고, BibTeX(.bib) 파일에서 인용 정보를 불러와 “\cite{}”로 자동 인용할 수 있습니다.

2. **Overleaf**  
   - **클라우드 기반 LaTeX 편집기**로, 웹브라우저만 있으면 어디서든지 `.tex` 문서를 작성·컴파일할 수 있습니다.  
   - 공동 작업이 용이해, 팀 프로젝트나 논문 공저 시 “버전 충돌” 걱정을 줄일 수 있습니다.  
   - `.bib` 파일을 업로드하면, Overleaf 프로젝트 내에서 **자동 참고문헌 생성**이 가능합니다.

3. **JabRef**  
   - 데스크톱에서 동작하는 **서지정보 관리 툴**로, BibTeX 파일(.bib)을 체계적으로 관리하기 위해 특화된 프로그램입니다.  
   - Google Scholar, PubMed, DBpia, ArXiv 등에서 찾은 논문의 정보를 자동으로 수집·정리하고, `.bib`에 저장할 수 있습니다.  
   - Overleaf와는 **파일 동기화**(手動 또는 클라우드 경유)가 가능해, 협업 환경에서도 원하는 문헌 정보를 즉시 공유 가능합니다.

이 세 도구를 연동하면, “내 PC에서 JabRef로 문헌을 정리” → “Overleaf로 .bib 업로드 및 공동 작성” → “LaTeX에서 \cite{}로 인용”이 모두 유기적으로 돌아가게 됩니다.

---

## 2. 준비 사항 & 기본 설치

1. **LaTeX 환경**  
   - 로컬 PC(Windows/Mac/Linux)에 TeX Live나 MiKTeX 같은 LaTeX 디스트리뷰션을 설치하면, 오프라인에서도 컴파일이 가능합니다.  
   - 그러나 Overleaf를 쓴다면, 브라우저만 있으면 되므로 꼭 로컬에 설치할 필요는 없습니다(선택사항).

2. **Overleaf 계정**  
   - [Overleaf 홈페이지](https://www.overleaf.com/)에서 회원가입 후, 무료 플랜으로 시작할 수 있습니다.  
   - 개인 프로젝트, 소규모 공동 작업 등에는 무료 버전도 충분합니다(프로 플랜은 히스토리 보관, 비공개 작업 등 추가 기능 지원).

3. **JabRef 설치**  
   - [JabRef 공식 사이트](https://www.jabref.org/)에서 OS별 설치 파일을 받을 수 있습니다.  
   - 설치 후 실행하면, 기본적으로 하나의 “라이브러리(.bib 파일)”를 만들거나 열어서 문헌 정보를 등록하게 됩니다.

4. **웹브라우저 확장 or 다른 검색**  
   - JabRef 자체에서도 논문 검색(온라인 문헌 가져오기)을 지원합니다.  
   - Google Scholar, DBpia, PubMed, ArXiv 등에서 BibTeX 파일을 **직접 내려받아서** JabRef에 추가하는 방법도 있습니다.

---

## 3. JabRef를 이용한 서지정보 관리

### 3.1 새로운 라이브러리(.bib) 만들기

1. JabRef 실행 → `File > New library` 선택.  
2. 원하는 이름(ex: `my_references.bib`)으로 저장.  
3. 화면 좌측 패널에 새 라이브러리가 생성됩니다.

**팁**: 프로젝트(논문)별로 .bib 파일을 여러 개 만들 수도 있지만, 보통 하나의 마스터 라이브러리를 만들어두고, 필요한 레퍼런스만 추출(Export)하는 방식을 많이 씁니다.

### 3.2 문헌 추가하기 (수동 & 자동)

- **(1) 수동 추가**  
  1. 상단 메뉴 “+” 아이콘 클릭 → 레퍼런스 타입 선택(@article, @book, @inproceedings 등).  
  2. 제목, 저자, 연도, 저널명, 페이지 등 메타데이터를 직접 입력.  
  3. BibTeX 키(예: kim2023Deep)는 자동으로 생성되지만, 원하는 규칙으로 수정도 가능합니다.

- **(2) 자동 추가**  
  1. Google Scholar 등에서 검색 후, **BibTeX로 내보내기**를 선택(“인용” 버튼 → BibTeX).  
  2. 다운로드된 `.bib` 파일(혹은 일부 텍스트)을 JabRef에 드래그앤드롭하면, 자동으로 새로운 레퍼런스가 추가됩니다.  
  3. JabRef 상단의 “Web Search” 기능(또는 DOI, ISBN 검색)을 이용하면 JabRef 자체에서 문헌 정보를 불러올 수 있습니다.

### 3.3 레퍼런스 관리 & 태깅

- **폴더(그룹) 기능**: JabRef의 왼쪽 패널에서 그룹을 만들고, 서로 다른 연구 주제별로 문헌을 나눠 관리할 수 있습니다(예: “Computer Vision”, “NLP”, “통계학” 등).  
- **키워드 태그**: 매 레퍼런스에 태그나 노트를 붙여두면, 특정 키워드로 쉽게 검색이 가능합니다(예: “#DeepLearning”, “#SurveyPaper”).  
- **파일 첨부**: PDF 원문 파일을 JabRef에 첨부(링크)해둘 수도 있습니다. 클릭 한 번으로 PDF 뷰어로 열리는 구조를 만들 수 있어, 자료 접근성이 향상됩니다.

### 3.4 Overleaf와 동기화(수동/자동)

- **수동 업로드**:  
  1. JabRef에서 “File > Export”로 현재 라이브러리를 `.bib` 형식으로 저장합니다.  
  2. Overleaf 프로젝트에 접속하여, “Upload” 버튼으로 `.bib` 파일을 업로드합니다.  
  3. Overleaf 상에서 `.tex` 파일과 `.bib`가 같은 프로젝트 내에 있으면, `\bibliography{my_references}` 식으로 연동 가능합니다.

- **클라우드 드라이브 연동**:  
  - Dropbox, Google Drive 등과 Overleaf를 연결해두면, 로컬에 있는 `.bib` 파일도 동기화할 수 있습니다(Overleaf → Account Settings → Integrations).  
  - JabRef에서 수정 → 클라우드 폴더와 자동 동기화 → Overleaf에서 `.bib` 변경사항 인식. (단, 플랜에 따라 동기화 간격이 다를 수 있음)

---

## 4. Overleaf에서 BibTeX를 활용한 참고문헌 자동화

### 4.1 기본 LaTeX 구조

**예시: main.tex**

```latex
\documentclass{article}
\usepackage[utf8]{inputenc}

\title{BibTeX & JabRef & Overleaf Test}
\author{Your Name}
\date{\today}

\begin{document}
\maketitle

이 문서에서 \LaTeX\ 과 BibTeX를 이용해 참고문헌을 관리합니다.
간단히 테스트해보면, 다음과 같이 인용할 수 있습니다:
\cite{kim2023Deep}.

\bibliographystyle{plain}
\bibliography{my_references}  % .bib 파일 이름(확장자 없이)
\end{document}
```

- `\bibliographystyle{plain}`: 참고문헌 표기 형식을 지정하는 명령어(plain, abbrv, alpha, IEEEtran 등 다양함).  
- `\bibliography{my_references}`: 현재 Overleaf 프로젝트에 업로드된 `my_references.bib` 파일을 가리킴(“.bib” 확장자는 제외).

### 4.2 Overleaf 프로젝트 셋업

1. **새 프로젝트 만들기**: Overleaf 대시보드에서 “New Project > Blank Project” 선택.  
2. **파일 업로드**:  
   - `main.tex`, `my_references.bib` 두 파일을 업로드합니다.  
   - 디렉토리 구조를 원하는 대로 설정해도 되지만, `.bib` 파일 경로를 `\bibliography{}`에 맞춰줘야 합니다.
3. **컴파일**: 우측 상단 “Recompile” 버튼을 누르면, LaTeX 문서가 빌드되며, 참고문헌 목록이 자동 생성됩니다.

**주의**: BibTeX를 쓸 때는 보통 **두 번 이상** 컴파일해야 인용번호와 레퍼런스가 정리됩니다. Overleaf에서는 자동으로 2회 이상 컴파일해주지만, 오류가 있으면 “Recompile”을 한 번 더 눌러주는 것을 권장합니다.

### 4.3 공동 작업 & 코멘트

- Overleaf 상에서 팀원들을 초대하면, 동시에 `.tex` 내용을 수정할 수 있습니다.  
- `.bib` 파일도 함께 편집 가능(단, BibTeX 문법이 깨지지 않도록 조심!).  
- 큰 수정이 있을 때는 **JabRef**에서 먼저 정리하고, `.bib`를 다시 업로드하는 방식을 추천합니다.

---

## 5. 실제 인용 예시: JabRef → Overleaf

1. **JabRef에서 논문 추가**  
   ```bibtex
   @article{kim2023Deep,
     title     = {Deep Learning for Text Classification},
     author    = {Kim, Min-jun and Lee, Soyeon},
     journal   = {AI & NLP Review},
     volume    = {15},
     number    = {2},
     pages     = {45-59},
     year      = {2023}
   }
   ```
2. **my_references.bib에 저장**  
   - JabRef에서 저장하거나, 내보내기(Export)로 `.bib` 파일을 갱신.
3. **Overleaf에 업로드**  
   - `my_references.bib` 파일 교체 업로드 (기존 파일을 덮어쓰기).  
   - Overleaf에서 자동으로 변경사항 인식.
4. **본문에서 인용**  
   ```latex
   ... \cite{kim2023Deep} ... 
   ```
5. **참고문헌 자동 생성**  
   - `\bibliographystyle{plain}` + `\bibliography{my_references}`로 인용 목록이 자동 생성됨.

---

## 6. BibTeX & LaTeX 사용 시 주의사항

1. **BibTeX 키 충돌**:  
   - 서로 다른 두 문헌이 같은 BibTeX 키(예: `kim2023Deep`)를 가지면 혼동이 발생합니다.  
   - JabRef는 보통 키를 자동 생성해주지만, 필요에 따라 **`author_year_title`** 형식으로 수정해 주세요.

2. **LaTeX 특수문자 처리**:  
   - 제목이나 저자명에 `&`, `%`, `#`, `_` 등의 특수문자가 들어가면 LaTeX 에러가 발생합니다.  
   - 예: `title = {Deep & Wide}` → `title = {Deep \& Wide}` 처럼 **이스케이프** 필요.

3. **인코딩(UTF-8) 설정**:  
   - 한글 문헌이 많은 경우, `\usepackage[utf8]{inputenc}` 및 BibTeX 설정도 UTF-8로 통일해야 글자 깨짐을 방지할 수 있습니다.

4. **\bibliographystyle** 선택**:**  
   - `plain`, `abbrv`, `alpha` 등 기본 스타일 외에도, IEEE, APA, Chicago 등 원하는 학술지 규정에 맞는 스타일이 있을 수 있습니다.  
   - 예: `\bibliographystyle{IEEEtran}` → IEEE 형식 인용으로 변경.  
   - 투고 저널마다 맞춤형 `.bst` 파일을 제공하기도 합니다.

5. **캡션, 피겨, 표와의 호환**:  
   - 종종 “Figure 1에서 보듯이 [1], ...” 식으로 인용할 때, 문맥에 맞게 LaTeX 문법을 조절해야 합니다.  
   - `\citep{...}`, `\citet{...}` 등 별도의 인용 스타일 매크로(natbib, biblatex) 사용 시 문서 유형에 따라 달라지므로 주의하세요.

---

## 7. 고급 기능 & 협업 팁

1. **JabRef의 ‘Automatic File Renaming’**  
   - 논문 PDF를 “저자-년도-제목.pdf” 형태로 자동 변환하여 정리해주는 기능이 있습니다(“Preferences > Import” 탭).  
   - 문서 관리에 통일성을 부여할 수 있어 편리합니다.

2. **Overleaf의 Git 연동**  
   - 유료 플랜(프로)에서는 Overleaf와 Git을 연동하여, `.tex`, `.bib` 파일 변화를 버전별로 추적이 가능합니다.  
   - 대규모 프로젝트나 장기 연구에 특히 유용합니다.

3. **BibLaTeX & Biber**  
   - 전통적인 BibTeX 대신, **BibLaTeX**(보다 유연하고 확장 가능한 방식)을 사용하는 프로젝트도 있습니다.  
   - Overleaf에서 `biber` 컴파일 옵션을 활성화하면, 보다 상세한 필드(예: `url`, `doi`, `urldate`)도 자동 처리할 수 있습니다.

4. **맞춤형 검색 필터**  
   - JabRef는 검색창에 특정 연도(예: year=2023), 저자(author="Kim"), 태그(#DeepLearning) 등으로 필터링이 가능합니다.  
   - 다량의 논문을 관리할 때, 검색 규칙을 잘 써먹으면 **원하는 문헌을 빠르게 찾기** 쉬워집니다.

---

## 8. 마무리 및 다음 단계

**LaTeX + JabRef + Overleaf** 조합은 논문·학위 논문·학술 보고서 작성에서 서지정보 정리의 **최고 효율**을 보장합니다.

- **핵심 요약**  
  1. **JabRef**로 문헌 메타데이터를 간편히 수집·정리 → `.bib`로 관리  
  2. **Overleaf**에서 `.tex`와 `.bib` 파일을 연동해, 공동 작업 및 자동 인용 처리  
  3. 인용 스타일 변경(예: IEEE, APA)도 LaTeX 한 줄 교체로 쉽게 해결

---

## 참고링크

- [JabRef 공식 홈페이지](https://www.jabref.org/)  
- [Overleaf 공식 홈페이지](https://www.overleaf.com/)  
- [LaTeX Project](https://www.latex-project.org/)  
- [BibTeX 공식 FAQ](http://www.bibtex.org/FAQ/)  

---
