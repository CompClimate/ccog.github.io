---
title: "Predicting Pacific fisheries"
excerpt: "Using Deep Learning to forecast marine fishery indicators in the North Pacific"
header:
    teaser: /assets/images/GRU_AbRec.png
featured_figure:
    image: /assets/images/GRU_AbRec.png
    caption: "Correlation maps of SST anomalies on the first Kernel Principal Component (PC) of Abundance (a) and on the second PC of Abundance (b). The same has been done for the Recruitment (c), (d)."

code: "https://github.com/maikejulie/DNN4Cli/tree/main/THOR/Step1"
people:
  - name: "Gian Giacomo Navarra"
    ccog: true
  - name: "Maike Sonnewald"
    ccog: true
  - name: "Yi Deng"
  - name: "Giovanni Liguori"
  - name: "Emanuele Di Lorenzo"
---

## Using Deep Learning to forecast marine fishery indicators in the North Pacific

Several studies have documented the strong link between North Pacific marine populations and climate variability. Yet, it remains unclear the extent to which these relations lead to improved forecasts of ecosystems. Using a deep learning tool (neural network) and a database of 125 biological timeseries from the Japan Research and Education Agency, we explored the extent to which physical predictability leads to multi-year prediction of dominant fisheries indicators. We have found that the Encoder-Decoder (ED) deep learning model was able to reproduce the testing data with a significant skill up to 4 years of lead time. To train the model we have used a set of physical variables, specifically we consider the SST and SSH for the all North Pacific Basin. The results from the ED have been compared with the forecast obtained from a Linear Inverse model approach and the persistence of the fish indicators. The deep learning performed better than both LIM model and the persistence for leading time above 2 years for most of the stocks. The results show that the physical drivers, exerts a primary control on the forecast of the ecological timeseries. Also, we demonstrate the potential of deep learning model to deal with stock time series forecasting without the need of dimensionality reduction. The ability of deep learning tools in having a skill-full forecast further in the future, can represent a promising approach for many socio-economic communities in order to adapt to climate change.
