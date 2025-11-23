---
layout: default
title: Top
---

## はじめに

TomoDesign Worksは、地域文化の記録と発信を目的としたWebプロジェクトです。

TomoDesign Works preserves social fluctuations and cultural fragments as a record of the future through designs that incorporate ideas into their structures.

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

インターネット黎明期には、数多くの個人ホームページが存在していました。近年、それらは急速に姿を消しつつありますが、そこには極めてローカルで、かけがえのない情報が宿っていました。

In the early days of the Internet, there were many personal homepages. In recent years, they have been rapidly disappearing, but they once contained extremely local and irreplaceable information

私たちは、GitHub PagesとJekyllを用いて、再現性・公共性・意味論的構造を備えたテンプレート設計を実践しながら、地域文化とデザインを融合した情報発信のかたちを探求し続けています。
