## Sequence2Sequence Speech Transcription System | ASR System 

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
