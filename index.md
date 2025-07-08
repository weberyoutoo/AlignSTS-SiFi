<style>
.main-content {
  max-width: 90%;
  width: 90%;
  margin: auto;
}
table {
  width: 100%;
  table-layout: fixed;
}
table th, table td {
  word-wrap: break-word;
  font-size: 0.9em;
  text-align: center;
  min-width: 300px;
  padding: 8px;
}
audio {
  width: 100%;
  max-width: 300px;
}
</style>

# <center>Self-supervised Learning Speech-to-Singing Conversion Based on Information Perturbation Techniques</center>

<center>Wei-Hsuan Kao and Von-Wun Soo</center>
<center>National Tsing Hua University, Taiwan, R.O.C</center>

## Abstract
<div style="text-align: justify">The Speech-to-Singing (STS) conversion task aims to convert speech into singing that matches a target melody while preserving timbre and content. However, most existing works heavily rely on parallel speech-singing corpora, which are expensive and time-consuming to collect. In this paper, we propose a lightweight self-supervised STS framework built upon the AlignSTS architecture, incorporating novel information perturbation techniques to enhance performance. These perturbations are used to prevent the model from overfitting to specific features, hence improving generalization. Unlike previous methods that apply perturbations directly to the waveform, our approach imposes perturbations on low-level acoustic features and employs a SiFi-GAN vocoder to synthesize the perturbed voice.</div>

## Speech-to-Singing conversion samples

<!-- ===================================================Comparative analysis=================================================== -->
## Comparative analysis

**1. you're giving me a million reasons to let you go you're giving me a million reasons to quit the show**
<table>
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
      <td><audio controls src="wavs/speech-2.wav"></audio></td>
      <td><audio controls src="wavs/sing-2.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>All perturb</th>
      <th>NO perturb</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/all-perturb-2.wav"></audio></td>
      <td><audio controls src="wavs/no-perturb-2.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>only TP</th>
      <th>only PS</th>
      <th>only RR</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/only-tp-2.wav"></audio></td>
      <td><audio controls src="wavs/only-PS-2.wav"></audio></td>
      <td><audio controls src="wavs/only-RR-2.wav"></audio></td>
    </tr>
  </tbody>
</table>
<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>w/o TP</th>
      <th>w/o PS</th>
      <th>w/o RR</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/AlignSTS-SiFi-2.wav"></audio></td>
      <td><audio controls src="wavs/wo-PS-2.wav"></audio></td>
      <td><audio controls src="wavs/wo-RR-2.wav"></audio></td>
    </tr>
  </tbody>
</table>

**2. there's a fire starting in my heart reaching a fever pitch and bringing me out the dark**
<table>
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
      <td><audio controls src="wavs/speech-8.wav"></audio></td>
      <td><audio controls src="wavs/sing-8.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>All perturb</th>
      <th>NO perturb</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/all-perturb-8.wav"></audio></td>
      <td><audio controls src="wavs/no-perturb-8.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>only TP</th>
      <th>only PS</th>
      <th>only RR</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/only-tp-8.wav"></audio></td>
      <td><audio controls src="wavs/only-PS-8.wav"></audio></td>
      <td><audio controls src="wavs/only-RR-8.wav"></audio></td>
    </tr>
  </tbody>
</table>
<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>w/o TP</th>
      <th>w/o PS</th>
      <th>w/o RR</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/AlignSTS-SiFi-8.wav"></audio></td>
      <td><audio controls src="wavs/wo-PS-8.wav"></audio></td>
      <td><audio controls src="wavs/wo-RR-8.wav"></audio></td>
    </tr>
  </tbody>
</table>

**3. love me like you do lo lo love me like you do touch me like you do to to touch me like you do what are you waiting for**
<table>
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
      <td><audio controls src="wavs/speech-10.wav"></audio></td>
      <td><audio controls src="wavs/sing-10.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>All perturb</th>
      <th>NO perturb</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/all-perturb-10.wav"></audio></td>
      <td><audio controls src="wavs/no-perturb-10.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>only TP</th>
      <th>only PS</th>
      <th>only RR</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/only-tp-10.wav"></audio></td>
      <td><audio controls src="wavs/only-PS-10.wav"></audio></td>
      <td><audio controls src="wavs/only-RR-10.wav"></audio></td>
    </tr>
  </tbody>
</table>
<table>
  <thread>
    <tr>
      <th>perturbations</th>
      <th>w/o TP</th>
      <th>w/o PS</th>
      <th>w/o RR</th>
    </tr>
  </thread>
  <tbody>
    <tr>
      <td>wavs</td>
      <td><audio controls src="wavs/AlignSTS-SiFi-10.wav"></audio></td>
      <td><audio controls src="wavs/wo-PS-10.wav"></audio></td>
      <td><audio controls src="wavs/wo-RR-10.wav"></audio></td>
    </tr>
  </tbody>
</table>

<!-- ===================================================Main results=================================================== -->
## Main results
- **GT Mel:**  We convert the ground truth audio into Mel-spectrogram, and use HiFi-GAN to re-synthesis it back to audio. 
- **AlignSTS:** The supervised STS model which is trained on pairwise speech-singing data of GT-English.
- **AlignSTS-unpaired:** A rough self-supervised STS model, in which the AlignSTS model is trained using non-pairwise data **without** any perturbation.
- **AlignSTS-SVPT:** A self-supervised STS model that is similar to our framework but uses the information perturbation techniques proposed by [SVPT](https://speech2sing.github.io/).
- **AlignSTS-SiFi:** The self-supervised STS model proposed in this paper, which incorporates the AlignSTS architecture with SiFi-GAN-based information perturbations.

**1. you're giving me a million reasons to let you go you're giving me a million reasons to quit the show**
<table>
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
      <td><audio controls src="wavs/speech-2.wav"></audio></td>
      <td><audio controls src="wavs/sing-2.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
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

**2. there's a fire starting in my heart reaching a fever pitch and bringing me out the dark**
<table>
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
      <td><audio controls src="wavs/speech-8.wav"></audio></td>
      <td><audio controls src="wavs/sing-8.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
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
      <td><audio controls src="wavs/GT mel-8.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-8.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-SVPT-8.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-SiFi-8.wav"></audio></td>
    </tr>
  </tbody>
</table>

**3. love me like you do lo lo love me like you do touch me like you do to to touch me like you do what are you waiting for**
<table>
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
      <td><audio controls src="wavs/speech-10.wav"></audio></td>
      <td><audio controls src="wavs/sing-10.wav"></audio></td>
    </tr>
  </tbody>
</table>

<table>
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
      <td><audio controls src="wavs/GT mel-10.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-10.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-SVPT-10.wav"></audio></td>
      <td><audio controls src="wavs/AlignSTS-SiFi-10.wav"></audio></td>
    </tr>
  </tbody>
</table>
