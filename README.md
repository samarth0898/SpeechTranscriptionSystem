## Sequence2Sequence Speech Transcription System 

This repo contains a sequence to sequence speech transcription system based on an encoder, decoder and attention mechanism. The English alphabets are learnt from the input mel frequency cepstral coefficients. (need to be completed)

### Prototyping Attention Mechanism
### Attention MAP 

Naive learning of input output correspondance using a K,Q,V attention mechanism between the encoder and decoder 

![Alt Text](https://github.com/samarth0898/SpeechTranscriptionSystem/blob/master/code/attention.gif)

Objectives of this work 

- Setup and encoder, decoder and attention based system to build correspondance between input MFCC and phonemes 
- Encoder synchrony and rate principles in encoder setup 
- Bidirectional LSTM cell / Pyramidal LSTM cell 


Training regimes 
- Teacher forcing mechanism 
- pack-padding variable length data 
- 



### Description of the input 
40-dimensional log-mel filter bank features were computed every 10ms and used as the acoustic inputs to the listener.


The encoder used is a pyramidal-BiLSTM for matching the input rate and the speech transcription rate which is about 8:1. 
This model is sigificantly influenced by the LAS paper 
LAS: Chan, William, et al. "Listen, attend and spell." arXiv preprint arXiv:1508.01211 (2015).

[REF: B. Raj, Deep Learning Carnegie Mellon University]
The pBLSTM is a variant of Bi-LSTMs that downsamples sequences by a factor of 2 by concatenating
adjacent pairs of inputs before running a conventional Bi-LSTM on the reduced-length sequence. So, given
an input vector sequence X0, X1, X2, X3, . . . XN−1, the pBLSTM first concatenates adjacent pairs of vectors
as [X0, X1], [X2, X3], . . . [XN−2, XN−1], and then computes a regular BiLSTM on the reshaped input.

-) Initial Bi-LSTM 
-) 3x Pyramidal Bi-LSTM 