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
<!-- Source: M1 -->
<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmoke; display: table;">
          <thead>
            <tr>
              <th style="width: 25%">Source Speaker</th>
              <th style="width: 25%">Target Speaker</th>
              <th style="width: 25%">Flowvae-VC</th>
              <th style="width: 25%">Flowvae-VC2</th>
            </tr>
          </thead>
          
          <!-- M1 to M -->
          <tbody>
            <tr>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/source/p283_270.wav" type="audio/wav" />
                </audio>
              </td>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/target/p237_259.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc1/3.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc2/3.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/source/p314_110.wav" type="audio/wav" />
                </audio>
              </td>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/target/p276_109.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc1/7.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc2/7.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td rowspan="7" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/source/p286_119.wav" type="audio/wav" />
                </audio>
              </td>
              <td rowspan="7" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/target/p374_032.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc1/9.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc2/9.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/source/p279_136.wav" type="audio/wav" />
                </audio>
              </td>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/target/p283_275.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc1/1.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc2/1.wav" type="audio/wav" />
                </audio>
              </td>
            </tr>

            <tr>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/source/p269_274.wav" type="audio/wav" />
                </audio>
              </td>
              <td rowspan="4" style="vertical-align: top;">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/target/p251_240.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc1/19.wav" type="audio/wav" />
                </audio>
              </td>
              <td style="width: 25%">
                <audio id="player" controls style="width: 100%;">
                    <source src="audio/flowvaevc2/19.wav" type="audio/wav" />
                </audio>
              </td>
           </tr>
          </tbody>
        </table>
    </div>
</div>

<p></p>
