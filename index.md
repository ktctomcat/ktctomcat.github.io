---
layout: default
title: Top
---

## はじめに

TomoDesign Worksは、構造に思想を宿すデザインを通じて、社会のゆらぎや文化の断片を来への記録として残しています。

<img id="rand-img" alt="トップ画像">

<script>
    (function() {
        const images = [];
        for (let i = 1; i <= 10; i++) {
            // 3桁ゼロ埋め (001, 002, …)
            const num = String(i).padStart(3, '0');
            images.push(`{{ '/assets/img/top/top-img-${num}.jpg' | relative_url }}`);
        }

        const pick = images[Math.floor(Math.random() * images.length)];
        document.getElementById('rand-img').src = pick;
    })();
</script>

インターネットの普及初期に数多く存在していた個人ホームページが、近年急速に姿を消しつつあります。  
しかし、そこには極めてローカルで、かけがえのない情報が宿っていました。

私たちは、GitHub PagesとJekyllを用いて、再現性・公共性・意味論的構造を備えたテンプレート設計を実践しながら、地域文化とデザインを融合した情報発信のかたちを探求し続けています。
