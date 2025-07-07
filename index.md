# <center>Self-supervised Learning Speech-to-Singing Conversion Based on Information Perturbation Techniques</center>

<center>Wei-Hsuan Kao and Von-Wun Soo</center>

<center>National Tsing Hua University, Taiwan, R.O.C</center>

## Abstract
The Speech-to-Singing (STS) conversion task aims to convert speech into singing that matches a target melody while preserving timbre and content. However, most existing works heavily rely on parallel speech-singing corpora, which are expensive and time-consuming to collect. In this paper, we propose a lightweight self-supervised STS framework built upon the AlignSTS architecture, incorporating novel information perturbation techniques to enhance performance. These perturbations are used to prevent the model from overfitting to specific features, hence improving generalization. Unlike previous methods that apply perturbations directly to the waveform, our approach imposes perturbations on low-level acoustic features and employs a SiFi-GAN vocoder to synthesize the perturbed voice.
