---
title: "Physics-driven and explainable AI for BNNs"
excerpt: "Toward trustworthy predictions of ocean dynamics"
header:
    teaser: "https://agupubs.onlinelibrary.wiley.com/cms/asset/342c6f7c-660a-41cb-ad5a-de08c542a2ca/jame21717-fig-0001-m.jpg"
featured_figure:
    image: "https://agupubs.onlinelibrary.wiley.com/cms/asset/342c6f7c-660a-41cb-ad5a-de08c542a2ca/jame21717-fig-0001-m.jpg"
learn_more: "https://doi.org/10.1029/2022MS003162"
code: "https://github.com/maikejulie/DNN4Cli/tree/main/THOR/BayesianApproach"
people:
  - name: "Mariana C. A. Clare"
    ccog: true
  - name: "Maike Sonnewald"
    ccog: true
  - name: "Redouane Lguensat"
  - name: "Julie Deshayes"
  - name: "V. Balaji"
  
---

## Explainable Artificial Intelligence for Bayesian Neural Networks: Toward Trustworthy Predictions of Ocean Dynamics

The trustworthiness of neural networks is often challenged because they lack the ability to express uncertainty and explain their skill. This can be problematic given the increasing use of neural networks in high stakes decision-making such as in climate change applications. 

We address both issues by successfully implementing a Bayesian Neural Network (BNN), where parameters are distributions rather than deterministic, and applying novel implementations of explainable AI (XAI) techniques. The uncertainty analysis from the BNN provides a comprehensive overview of the prediction more suited to practitioners' needs than predictions from a classical neural network. Using a BNN means we can calculate the entropy (i.e., uncertainty) of the predictions and determine if the probability of an outcome is statistically significant. To enhance trustworthiness, we also spatially apply the two XAI techniques of Layer-wise Relevance Propagation (LRP) and SHapley Additive exPlanation (SHAP) values. 

These XAI methods reveal the extent to which the BNN is suitable and/or trustworthy. Using two techniques gives a more holistic view of BNN skill and its uncertainty, as LRP considers neural network parameters, whereas SHAP considers changes to outputs. We verify these techniques using comparison with intuition from physical theory. The differences in explanation identify potential areas where new physical theory guided studies are needed.

**What's new:**
- Novel use of a Bayesian Neural Network (BNN) to quantify uncertainty in ocean dynamical regime classifications, giving a holistic prediction
- Explaining the skill of a BNN using two techniques originating from two different classes of explainable AI: SHapley Additive exPlanation (SHAP) and Layer-wise Relevance Propagation (LRP)
- Trustworthiness is evaluated by comparing similarities and differences between SHAP and LRP explanations with intuition from physical theory