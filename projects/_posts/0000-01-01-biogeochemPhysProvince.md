---
title: "North Atlantic physical and biogeochemical provinces"
excerpt: "Objective data mining of North Atlantic physical and biogeochemical data"
header:
    teaser: /assets/images/provinces.png
featured_figure:
    image: /assets/images/provinces.png
    caption: "Provinces (colours) determined using NEMI on data from Jenniges et al. (in prep). Left: spatial 3D representation. Right: Provinces illustrated in embedded space."

code: "https://github.com/maikejulie/DNN4Cli/tree/main/THOR/Step1"
people:
  - name: "Yvonne Jenniges"
    ccog: true
  - name: "Maike Sonnewald"
    ccog: true
tags:
  - ocean
  - data mining
  - observations
  - probabilistic ML
---

## Towards objective data mining: An example on 3D North Atlantic physical and biogeochemical data

The ocean plays a vital role for our climate system through its ability to, for example, store and redistribute heat and carbon. Despite the oceans' importance, key insight to predict its future variability is lacking. This is because ocean data is sparse and it is governed by complex, nonlinear and chaotically interacting components on timescales spanning seconds to millennia.  Here, we exploit growing availability of data from diverse sources and present a righteous and objective methodology for detecting patterns in complex data. Our method uses manifold-based embedding to reduce dimensionality and strengthen statistical associations as well as density-based clustering and field-specific utility enhancement. A central and inherent challenge of conventional methods, such as unsupervised machine learning, is validation. This is because an objective "truth" to compare against is missing. We present a combination of external and internal validation methods to assess how well different clustering algorithms perform both on original and embedded data. Key findings include that clusterings on the embedding outperform clusterings on the original data-space, and that various validation methodologies (Silhouette, Davies-Bouldin and Calinski-Harabasz) do not consistently agree and converge on parameter choices. This emphasizes the need for applying several internal and external validation methods which has rarely been done in literature.
