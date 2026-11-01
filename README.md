# DA-ICL: Distribution-Aware In-Context Learning for Arabic ASR Error Correction

Companion repository for the paper published in IEEE Access:
https://ieeexplore.ieee.org/document/11601033  (DOI: 10.1109/ACCESS.2026.3711662)

## Overview
Two-stage framework for Arabic ASR:
1. HuBERT fine-tuned on Common Voice Arabic (baseline WER 19.3%).
2. DA-ICL: few-shot prompting of Aya-23-8B using examples selected from a
   taxonomy of ASR error types (phonetic confusions, morpho-orthographic errors).
   WER reduced to 9.6%.
3. LoRA adaptation of HuBERT for domain shift: out-of-domain WER 67% -> 24%.

## Results (Common Voice Arabic)
| System | WER |
|---|---|
| HuBERT (fine-tuned) | 19.3% |
| Whisper-large (zero-shot) | 47.49% |
| Whisper-large (LoRA) | 37.89% |
| HuBERT + DA-ICL | 9.6% |


## Citation
@ARTICLE{11601033,
  author={Sbih, Rima and Jafar, Assef and Kazem, Ali},
  journal={IEEE Access}, 
  title={DA-ICL: Distribution-Aware In-Context Learning for Arabic Automatic Speech Recognition Error Correction}, 
  year={2026},
  volume={14},
  number={},
  pages={106917-106926},
  keywords={Automatic speech recognition;Licenses;Modeling;Large language models;LoRa;Nuclear facility regulation;Speech;Tuning;Learning (artificial intelligence);Context;Arabic speech recognition;large language models;HuBERT;in-context learning;distribution-aware in-context learning;parameter-efficient fine-tuning;low-rank adaptation;error correction},
  doi={10.1109/ACCESS.2026.3711662}}
