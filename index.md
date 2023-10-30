# FLOW-VAE VC2: RETHINKING CONDITIONAL METHODS FOR FLOW-VAE VC

<font size="5">Rongxiu Zhong, Shilei Zhang, Yanan Chen,Yong Ma, Ying Liu, Huibao Yang, Junlan Feng </font>

## Abstract

Voice conversion (VC) seeks to modify one speaker’s voice to generate speech as if it came from another speaker. It is challenging especially when source and target speakers are unseen during training (zero-shot VC). Our previous work Flow-VAE VC is an end-to-end system for zero-shot tasks, which processing directly on the raw audio waveform, but it still needs pre-trained model to extract the speaker embedding as conditional input and has an insurmountable gap between real and converted speech. To overcome these limitations, we propose Flow-VAE VC2, which is an improved version of Flow-VAE VC incorporating three new techniques: improved speaker encoder network(RawNet3 network), and improved generator(MS-iSTFT decoder), and improved objective(a supervised contrastive loss and AAM-softmax loss). We examined the performance of the proposed methods on the zero-shot VC task. An objective evaluation demonstrates that the proposed methods effectively preserve the source linguistic content, and  achieve much higher generation speed. A subjective evaluation shows that Flow-VAE VC2 outperforms Flow-VAE VC in terms of both naturalness and speaker similarity.

<p></p>

## Audio Demos

This page contains voice conversion samples for FLOW-VAE VC2 applied to audio files from the [VCTK Corpus](https://datashare.ed.ac.uk/handle/10283/3443).
We provide comparisons with other models: FLOW-VAE VC


### Navigation

* [Seen-to-Seen Voice Conversion](#seen-to-seen-voice-conversion)
* [Unseen-to-Unseen Voice Conversion](#unseen-to-unseen-voice-conversion)

<p></p>

### audio samples coming soon
