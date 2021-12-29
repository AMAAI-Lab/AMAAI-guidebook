# nnAudio
nnAudio is an audio processing toolbox using PyTorch convolutional neural network as its backend. By doing so, spectrograms can be generated from audio on-the-fly during neural network training and the Fourier kernels (e.g. or CQT kernels) can be trained. [Kapre](https://github.com/keunwoochoi/kapre) has a similar concept in which they also use 1D convolutional neural network to extract spectrograms based on [Keras](https://keras.io).

Other GPU audio processing tools are [torchaudio](https://github.com/pytorch/audio) and [tf.signal](https://www.tensorflow.org/api_docs/python/tf/signal). But they are not using the neural network approach, and hence the Fourier basis can not be trained. As of PyTorch 1.6.0, torchaudio is still very difficult to install under the Windows environment due to `sox`. nnAudio is a more compatible audio processing tool across different operating systems since it relies mostly on PyTorch convolutional neural network. The name of nnAudio comes from `torch.nn`

## Installation
`pip install git+https://github.com/KinWaiCheuk/nnAudio.git#subdirectory=Installation`

or

`pip install nnAudio==0.3.0`

## Documentation
https://kinwaicheuk.github.io/nnAudio/index.html

## Comparison with other libraries
| Feature | [nnAudio](https://github.com/KinWaiCheuk/nnAudio) | [torch.stft](https://github.com/pytorch/pytorch/blob/master/aten/src/ATen/native/SpectralOps.cpp) | [kapre](https://github.com/keunwoochoi/kapre) | [torchaudio](https://github.com/pytorch/audio) | [tf.signal](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/python/ops/signal) | [torch-stft](https://github.com/pseeth/torch-stft) | [librosa](https://github.com/librosa/librosa) |
| ------- | ------- | ---------- | ----- | ---------- | ---------------------------- | ---------- | ------- |
| Trainable | ✅ | ❌| ✅ | ❌ | ❌ | ✅ | ❌ |
| Differentiable | ✅  | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ |
| Linear frequency STFT| ✅  | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Logarithmic frequency STFT| ✅  | ❌ | ✅ | ❌ | ❌ | ❌ | ❌ |
| Inverse STFT| ✅  | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| Griffin-Lim| ✅  | ❌ | ❌ | ✅ | ✅ | ❌ | ✅ |
| Mel | ✅ | ❌ | ✅ | ✅ | ✅ | ❌ | ✅ |
| MFCC | ✅  | ❌ | ❌ | ✅| ✅ | ❌ | ✅ |
| CQT | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |
| Gammatone | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| CFP<sup>1</sup> | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| GPU support | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ |

✅: Fully support    ☑️: Developing (only available in dev version)    ❌: Not support

<sup>1</sup> [Combining Spectral and Temporal Representations for Multipitch Estimation of Polyphonic Music](https://ieeexplore.ieee.org/document/7118691)
