---
layout: page
title: NS-CUK Weekly Seminar on 2022
permalink: /seminar/2022/
image: CUK_4Seasons.jpg
description: Archive of papers reviewed by members of the Network Science Lab at the Catholic University of Korea as part of the NS-CUK Weekly Seminar series
last_modified_at: 2025-01-03 15:30:00 +0900
---

<!-- ![image](https://github.com/NSLab-CUK/NSLab-CUK.github.io/assets/100113405/96ea07b1-9117-4436-9e78-5f554d6629a4) -->



This page is an archive for papers reviewed by members of the Network Science Lab, along with corresponding presentation materials, as part of the NS-CUK Weekly Seminar series. Launched in Fall 2022, this seminar series is intended to be a platform for the members of the Network Science Lab at the Catholic University of Korea to exchange insights and understanding of state-of-the-art AI methodologies and models for graph mining.

***

##### [This Year](https://nslab-cuk.github.io/seminar/)

***
### 2022

***

#### Dec 7th, 2022
{:.no_toc}

<details markdown="1">
  <summary>S.T. Nguyen, Review on "Complex Embeddings for Simple Link Prediction", ICML 2016</summary>
  <p align="center"><iframe src="https://docs.google.com/presentation/d/1qFuoZScaHHtu22RKHdh1Y4zCDNM0MfKv/edit?usp=sharing&ouid=108773870950556903410&rtpof=true&sd=true" width="90%" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe></p>
</details>

***

#### Dec 5th, 2022
{:.no_toc}

<details markdown="1">
  <summary>H.B. Kim, Review on "One-hot Encoding for Deep Learning (Part 2)"</summary>
</details>

***

#### Nov 30th, 2022
{:.no_toc}

<details markdown="1">
  <summary>S.T. Nguyen, Review on "Knowledge Graph Embedding by Translating on Hyperplanes", AAAI 2014</summary>
  <p align="center"><iframe src="https://docs.google.com/presentation/d/1HdZ6veXiobuuRr5DuKVQkO8WQht9yfEn/edit?usp=sharing&ouid=108773870950556903410&rtpof=true&sd=true" width="90%" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe></p>
</details>

***

#### Nov 28th, 2022
{:.no_toc}

<details markdown="1">
  <summary>H.B. Kim, Review on "One-hot Encoding for Deep Learning"</summary>
</details>

***

#### Nov 23rd, 2022
{:.no_toc}

<details markdown="1">
  <summary>S.T. Nguyen, Review on "Learning Role-based Graph Embeddings"</summary>
</details>

<details markdown="1">
  <summary>S.M. Lee, Review on "Basic on Graph Mining"</summary>
</details>

***

#### Nov 21st, 2022
{:.no_toc}

<details markdown="1">
  <summary>조세은, Review on "Deep Generative Models"</summary>
</details>

***

#### Nov 16th, 2022
{:.no_toc}

<details markdown="1">
  <summary>S.T. Nguyen, Review on "Directed Graph Embedding with Asymmetric Transitivity Preservation", AAAI 2019</summary>
  <p align="center"><iframe src="https://docs.google.com/presentation/d/1UygkwseY5Hr3oGrPoyGbVjhfj75F6NgW/edit?usp=sharing&ouid=108773870950556903410&rtpof=true&sd=true" width="90%" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe></p>
</details>

***

#### Nov 9th, 2022
{:.no_toc}

<details markdown="1">
  <summary>S.M. Lee, Review on "KNN (K nearest neighbors algorithm)"</summary>
</details>

<details markdown="1">
  <summary>S.T. Nguyen, Review on "MetaGraph2Vec: Complex Semantic Path Augmented Heterogeneous Network Embedding", PAKDD 2018</summary>
  <p align="center"><iframe src="https://docs.google.com/presentation/d/1REub9wC7h6txVbjdONFplU66tKF40-Cw/edit?usp=sharing&ouid=108773870950556903410&rtpof=true&sd=true" width="90%" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe></p>
</details>

***

#### Nov 7th, 2022
{:.no_toc}

<details markdown="1">
  <summary>조세은, Review on "Applications in Deep Learning"</summary>
</details>

***

#### Oct 31st, 2022
{:.no_toc}

<details markdown="1">
  <summary>조세은, Review on "Linear Factor Models"</summary>
</details>

***

#### Oct 21st, 2022
{:.no_toc}

<details markdown="1">
  <summary>S.M. Lee, Review on "Sequence Modeling: Recurrent and Recursive Nets and Regularization"</summary>
</details>

<details markdown="1">
  <summary>V.T. Hoang, Review on "Autoencoder and Machine Learning basics"</summary>
</details>





<script>
document.addEventListener("DOMContentLoaded", function() {
  // 모든 details 요소를 선택
  const detailsElements = document.querySelectorAll('details');

  detailsElements.forEach(details => {
    // 각 details 안의 iframe 찾기
    const iframe = details.querySelector('iframe');
    
    if (iframe) {
      // 원본 iframe의 src를 data-src 속성으로 저장
      iframe.setAttribute('data-src', iframe.src);
      iframe.src = ''; // iframe src 비워 로드 방지
    }

    // details가 열리고 닫힐 때 처리
    details.addEventListener('toggle', function() {
      const iframe = details.querySelector('iframe');
      if (!iframe) return;

      if (details.open) {
        // 열렸을 때 원래 주소를 iframe에 설정하여 로딩
        iframe.src = iframe.getAttribute('data-src');
      } else {
        // 닫혔을 때 src를 비워 iframe 로드 취소
        iframe.src = '';
      }
    });
  });
});
</script>
