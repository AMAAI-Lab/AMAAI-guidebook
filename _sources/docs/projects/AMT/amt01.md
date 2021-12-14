# Problem Formulation
Given a spectrogram $𝑋\in \mathbb{R}^{F \times T}$,
we want to obtain a posteriorgram $Y_{\text{post}}\in [0,1]^{88\times T}$ via a neural network model $Y_{\text{post}}=f(X)$.
The piano roll $Y\in \{0,1\}^{88\times T}$ can be obtained via applying a hard threshold on $Y_{\text{post}}$.

```{figure} ../../../images/amt_formulation.png
---
height: 150px
name: amt_formulation
---
The goal of AMT is to transform audio data into symbolic representations.
```