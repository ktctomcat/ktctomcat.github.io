---
layout: default
title: Top
---

## はじめに

TomoDesign Worksは、構造に思想を宿すデザインを通じて、社会のゆらぎや文化の断片を来への記録として残しています。

<img id="rand-img" alt="トップ画像">

<script>
  (function() {
    const images = [
      "{{ '/assets/img/top/top-img-001.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-002.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-003.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-004.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-005.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-006.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-007.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-008.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-009.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-010.jpg' | relative_url }}"
    ];
    const pick = images[Math.floor(Math.random() * images.length)];
    const img = document.getElementById('rand-img');
    img.src = pick;
  })();
</script>

インターネットの普及初期に数多く存在していた個人ホームページが、近年急速に姿を消しつつあります。  
しかし、そこには極めてローカルで、かけがえのない情報が宿っていました。

私たちは、GitHub PagesとJekyllを用いて、再現性・公共性・意味論的構造を備えたテンプレート設計を実践しながら、地域文化とデザインを融合した情報発信のかたちを探求し続けています。