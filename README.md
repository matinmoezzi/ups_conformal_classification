# An Uncertainty-Aware Pseudo-Label Selection Framework using Regularized Conformal Prediction
This codebase implements a novel pseudo-labeling based semi-supervised learning method which mitigates the poor performance of pseudo-labeling method. This work is based on these two papers and their codes:
- [Uncertainty Sets for Image Classifiers using Conformal Prediction](https://arxiv.org/pdf/2009.14193.pdf)
- [In Defense of Pseudo-Labeling: An Uncertainty-Aware Pseudo-Label Selection Framework for Semi-supervised Learning](https://arxiv.org/pdf/2101.06329.pdf)

The main contribution of this work is to employ the idea of the first paper into the second paper approach. To be specific, the first paper proposes an uncertainty quantification framework (RAPS) which wraps around any image classifier and outputs a predictive sets for each sample, representing the uncertainty of the model. The second paper proposes an algorithm (UPS) which modifies the high confidence selection process using estimating uncertainty; In fact, the proposed approach selects a subset of pseudo-labels based on both confidence and uncertainty prediction to reduce noisy data during training. This work incorporates the RAPS outputs into UPS to generate pseudo-labels with respect to predictive sets instead of hard pseudo-labeling.

## Google Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/matinmoezzi/ups_conformal_classification/blob/main/train-ups-raps.ipynb)
