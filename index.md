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

## Main results

### 1. 
you're giving me a million reasons to let you go you're giving me a million reasons to quit the show 
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

### 2. 
there's a fire starting in my heart reaching a fever pitch and bringing me out the dark 
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

### 3. 
love me like you do lo lo love me like you do touch me like you do to to touch me like you do what are you waiting for 
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
