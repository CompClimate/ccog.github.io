---
title: "Predicting ocean biomes remotely"
excerpt:  "Lessons from inferring plankton eco-provinces with remotely sensed data"
header:
    teaser: "assets/images/makaylaNN.png"
featured_figure: 
    image: "assets/images/ecopred.png"
    caption: Eco-provinces of summer and winder data. Top left shows ten eco-provinces in manifold space, with geographical projections to the right. Colours correspond to distinct biomes. Below, the same showing the uncertainty per point. Dark colours signify low uncertainty. 
code: "https://github.com/maikejulie/DNN4Cli"
people:
  - name: "Makayla McDevitt"
    ccog: true
  - name: "Maike Sonnewald"
    ccog: true
  - name: "Steph Dutkiewicz"

tags:
  - ocean
  - deep learning
  - probabilistic ML
  - unsupervised learning
  - policy
  - data mining
---

## Identifying and Predicting Eco-Provinces in the Global Ocean

Ecological marine provinces, "eco-provinces," represent coherent and ecologically meaningful regions in the global ocean in terms of biogeography. Marine ecosystems face increasing threats due to climate change and human activities, necessitating improved tools to identify and predict spatially explicit habitat information for ecosystem-based fisheries management. In two primary steps, this research presents 1) an unsupervised clustering algorithm to identify eco-provinces based on modeled phytoplankton functional type data, and 2) a prediction algorithm based on modeled fields observable from the ocean’s surface via satellites. Explainable AI (XAI) offers insight into the importance of each input feature in the neural network’s prediction. 
For Step 1, we utilize the Native Emergent Manifold Interrogation (NEMI) framework (Sonnewald, 2023) to identify eco-provinces based on phytoplankton functional type data from the Darwin Biogeochemistry model (Dutkiewicz et al., 2015). Entropy quantifies the uncertainty of eco-province identification. Input data consists of five functional type concentrations from a 22 year summer and winter mean spanning 1993-2015. Identified eco-provinces align with known biogeographical patterns, including expected seasonal shifts between diatom-dominated upwelling regions, and smaller functional types existing in oligotrophic gyres.
For prediction capabilities in Step 2, an ensemble MLP with latent space regularization predicts eco-provinces based on Darwin Biogeochemistry Model data. The input features are blue and green light irradiance reflectance, total phytoplankton concentration, and total chlorophyll concentration. A group or “ensemble” of 10 neural networks dedicated to the same optimization problem were employed in order to increase the robustness of the results. Averaging across the ensemble, the neural network version incorporating all four inputs achieved optimal performance with validation accuracy equal to 85%. XAI techniques identified the contribution of each input to the network’s prediction and provided insight into the origin of whether the prediction was correct or not. This prediction mechanism based on modeled data serves as a proof of concept for applications to novel satellite datasets, such as from NASA's Plankton, Aerosol, Cloud, ocean Ecosystem (PACE) mission. Compatibility with satellite data would allow for updated characterizations and predictions of spatially explicit habitat information, which then could be mapped to higher trophic level species distributions. Satellite-based ocean region characterization and prediction with the addition of information about species at higher trophic levels provides potential usefulness for ecosystem-based fisheries management.
