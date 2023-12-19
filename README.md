# Embeddings Translation using Geometric Loss

Peter Bowman-Davis and Kristof Reimann for Yale CPSC 488, research project for AI foundation models.

Extends on prior work of [VectorBridge](https://github.com/P-H-B-D/EmbeddingsTranslation) (Peter Bowman-Davis and Roshan Palakkal), we leverage geometric properties of embeddings spaces for the purpose of cross-model translation. 

We hypothesize that there is some high dimensional intrinsic structure of language that is learned during the training of different embeddings models. By measuring some of these properties, we hope to devise a loss function that is more performant than the simple loss function used in [VectorBridge](https://github.com/P-H-B-D/EmbeddingsTranslation). 

In this project, we attempt a variety of geometric measurements: 
- Linear measurements in ```linearAnalysis.ipynb```
- Local Linearity Estimation (LLE) in ```locallyLinearEmbedding.ipynb```
- Diffusion Curvature estimation in ```diffusionCurvature.ipynb```
- k-Means cross-model embeddings clustering with silhouette scoring in ```kMeans.ipynb```
- Random k-Means sampling for cross-model cluster invariance analysis in ```randomKMeans.ipynb```
- Training of the translation model ```translationModel.ipynb```
- Evaluation of a translation model across epochs using k-Means score in ```translationModelKMeansLoss.ipynb```
