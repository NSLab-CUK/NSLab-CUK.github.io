---
layout: page
title: NS-CUK Weekly Seminar
permalink: /seminar/
image: CUK_4Seasons.jpg
description: Archive of papers reviewed by members of the Network Science Lab at the Catholic University of Korea as part of the NS-CUK Weekly Seminar series
last_modified_at: 2025-04-02 15:30:00 +0900
---

<!-- ![image](https://github.com/NSLab-CUK/NSLab-CUK.github.io/assets/100113405/96ea07b1-9117-4436-9e78-5f554d6629a4) -->



This page is an archive for papers reviewed by members of the Network Science Lab, along with corresponding presentation materials, as part of the NS-CUK Weekly Seminar series. Launched in Fall 2022, this seminar series is intended to be a platform for the members of the Network Science Lab at the Catholic University of Korea to exchange insights and understanding of state-of-the-art AI methodologies and models for graph mining.

***

<h5>Previous Years</h5>

* [2025](https://nslab-cuk.github.io/seminar/2025/)
* [2024](https://nslab-cuk.github.io/seminar/2024/)
* [2023](https://nslab-cuk.github.io/seminar/2023/)
* [2022](https://nslab-cuk.github.io/seminar/2022/)

***
#### Jan 05th, 2026
{:.no_toc}

<details markdown="1">
  <summary>V.T. Hoang, Review on "MolTC: Towards Molecular Relational Modeling In Language Models", ACL 2024</summary>
  <p align="center"><iframe src="https://www.slideshare.net/slideshow/embed_code/key/uWCxyxY1i9boLO?hostedIn=slideshare&page=upload" width="90%" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"
style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen></iframe></p>
</details>

<details markdown="1">
  <summary>H.W. Kim, Review on "Shift-Robust Molecular Relational Learning with Causal Substructure", KDD 2023</summary>
  <p align="center"><iframe src="https://www.slideshare.net/slideshow/embed_code/key/tpayYmIqgSETzz?hostedIn=slideshare&page=upload" width="90%" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"
style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen></iframe></p>
</details>

<details markdown="1">
  <summary>J.H. Cho, Review on "A Plant-Wide Industrial Process Control Problem", Computers & chemical engineering 1993</summary>
  <p align="center"><iframe src="https://www.slideshare.net/slideshow/embed_code/key/i3aetTO4AKUQ0y?hostedIn=slideshare&page=upload" width="90%" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"
style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen></iframe></p>
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
