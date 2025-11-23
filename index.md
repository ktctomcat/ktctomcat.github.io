---
layout: default
title: Top
---

## はじめに

TomoDesign Worksは、地域文化の記録と発信を目的としたWebプロジェクトです。

<figure class="rand-image">
  <img id="rand-img" alt="ランダム画像">
  <figcaption>ランダム表示（クライアント側）</figcaption>
</figure>

<script>
  (function() {
    const images = [
      "{{ '/assets/img/top/top-img-001.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-002.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-003.jpg' | relative_url }}",
      "{{ '/assets/img/top/top-img-004.jpg' | relative_url }}",
    ];
    const pick = images[Math.floor(Math.random() * images.length)];
    const img = document.getElementById('rand-img');
    img.src = pick;
  })();
</script>

インターネット黎明期には、数多くの個人ホームページが存在していました。近年、それらは急速に姿を消しつつありますが、そこには極めてローカルで、かけがえのない情報が宿っていました。

私たちは、GitHub PagesとJekyllを用いて、再現性・公共性・意味論的構造を備えたテンプレート設計を実践しながら、地域文化とWeb技術の融合による情報発信のかたちを探求し続けています。