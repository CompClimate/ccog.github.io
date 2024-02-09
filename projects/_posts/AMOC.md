---
title: "The Importance of Architecture Choice in Deep Learning for Climate Applications"
excerpt:  "Can neural networks simulate climate?"
header:
    teaser: "assets/images/simonAMOC.png"
featured_figure: 
    image: "assets/images/simonAMOC.png"
code: "https://github.com/CompClimate/StommelBoxModel"
people:
  - name: "Simon Draeger"
    ccog: true
  - name: "Maike Sonnewald"
    ccog: true
tags:
  - ocean
  - deep learning
  - probabilistic ML
  - fundamental understanding
---
The Importance of Architecture Choice in Deep Learning for Climate Applications

Machine Learning has become a pervasive tool in climate science applications. However, current models fail to address nonstationarity induced by anthropogenic
alterations in greenhouse emissions and do not routinely quantify the uncertainty of proposed projections. In this paper, we model the Atlantic Meridional Overturning
Circulation (AMOC) which is of major importance to climate in Europe and the US East  Coast by transporting warm water to these regions, and has the potential for abrupt collapse. We can generate arbitrarily
extreme climate scenarios through arbitrary time scales which we then predict using neural networks. Our analysis shows that the AMOC is predictable using neural networks
under a diverse set of climate scenarios. Further experiments reveal that MLPs and Deep Ensembles can learn the physics of the AMOC instead of imitating its progression through
autocorrelation. An intriguing pattern of "spikes" before critical points of collapse in the AMOC casts doubt on previous analyses that predicted an AMOC collapse within this century.
Our results show that Bayesian Neural Networks perform poorly compared to more dense architectures and care should be taken when applying neural networks to nonstationary scenarios such as climate
projections. Further, our results highlight that big NN models like FourCastNet, ACE, and Neural GCMs might have difficulty in modeling global Earth System dynamics accurately and successfully applied in nonstationary
climate scenarios due to the physics being challenging for neural networks to capture.
