# Source Codes
AMAAI has developed different AMT models

## Spectrogram Reconstruction AMT
This model {cite}`cheuk2021effect` uses spectrogram reconstruction to boost transcription accuracy.

[source code](https://github.com/KinWaiCheuk/ICPR2020)  

```{figure} ../../../images/reconstruction_model.png
---
width: 700px
name: reconstruction_model
---
Model architecture for spectrogram reconstruction AMT
```

## ReconVAT
ReconVAT {cite}`ReconVAT` is a semi-supervised AMT framework. This work is an extension of previous work by combining both virtual adversarial training (VAT) {cite}`VAT_semi` and spectrogram reconstruction AMT {cite}`cheuk2021effect`.

[source code](https://github.com/KinWaiCheuk/ReconVAT)  
[demo](https://kinwaicheuk.github.io/ReconVAT/)


```{figure} ../../../images/ReconVAT_model.png
---
width: 700px
name: ReconVAT_model
---
Model architecture for ReconVAT
```

## Understanding AMT using attention mechanism
We tried to understand AMT using additive attention mechanism.

[source code](https://github.com/KinWaiCheuk/IJCNN2021.github.io)  
[demo](https://kinwaicheuk.github.io/IJCNN2021.github.io/)


```{figure} ../../../images/attention_AMT.png
---
width: 700px
name: attention_AMT
---
Model architecture for ReconVAT
```