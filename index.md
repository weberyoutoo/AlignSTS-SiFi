# <center>Self-supervised Learning Speech-to-Singing Conversion Based on Information Perturbation Techniques</center>

<center>Wei-Hsuan Kao and Von-Wun Soo</center>
<center>National Tsing Hua University, Taiwan, R.O.C</center>

## Abstract
<div style="text-align: justify">The Speech-to-Singing (STS) conversion task aims to convert speech into singing that matches a target melody while preserving timbre and content. However, most existing works heavily rely on parallel speech-singing corpora, which are expensive and time-consuming to collect. In this paper, we propose a lightweight self-supervised STS framework built upon the AlignSTS architecture, incorporating novel information perturbation techniques to enhance performance. These perturbations are used to prevent the model from overfitting to specific features, hence improving generalization. Unlike previous methods that apply perturbations directly to the waveform, our approach imposes perturbations on low-level acoustic features and employs a SiFi-GAN vocoder to synthesize the perturbed voice.</div>

## Speech-to-Singing conversion samples

### Main results
Here, we show the original speech, the target singing, and the results produced by each model.

#### 1. 
<table class="small">
  <thread>
    <tr>
      <th>source</th>
      <th>Speech</th>
      <th>Singing</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/speech-2.wav" style="width: 70px;"></audio></td>
      <td><audio controls src="wavs/sing-2.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table class="small">
  <thread>
    <tr>
      <th>source</th>
      <th>GT mel</th>
      <th>AlignSTS</th>
      <th>AlignSTS-SVPT</th>
      <th>AlignSTS-SiFi</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/GT mel-2.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-2.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-SVPT-2.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-SiFi-2.wav"></audio></td>
    </tr>
  </tbody>
</table>
