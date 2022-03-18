---
language: 
- en
- fr
- ro
- de
datasets:
- c4
tags:
- summarization
- translation

license: apache-2.0
---

[Google's T5](https://ai.googleblog.com/2020/02/exploring-transfer-learning-with-t5.html) 

## PreTraining

The model was pre-trained on a on a **multi-task mixture of unsupervised (1.) and supervised tasks (2.)**.
Thereby, the following datasets were being used for (1.) and (2.):

1. **Datasets used for Unsupervised denoising objective**:

- Pretraining Dataset: [C4](https://huggingface.co/datasets/c4)

2. **Datasets used for Supervised text-to-text language modeling objective**

- Sentence acceptability judgment
  - (CoLA (Warstadt et al., 2018))
- Sentiment analysis (SST-2 (Socher et al., 2013))
- Paraphrasing/sentence similarity (MRPC (Dolan and Brockett, 2005), STS-B (Cer
et al., 2017), QQP (Iyer et al., 2017))
- Natural language inference (MNLI (Williams et al., 2017), QNLI (Rajpurkar et al.,
2016), RTE (Dagan et al., 2005), CB (De Marneff et al., 2019))
- Coreference resolution (WNLI and WSC (Levesque et al., 2012))
- Sentence completion (COPA (Roemmele et al., 2011))
- Word sense disambiguation (WIC (Pilehvar and Camacho-Collados, 2018))
- Question answering (MultiRC (Khashabi et al., 2018), ReCoRD (Zhang et al., 2018),
BoolQ (Clark et al., 2019))

## All T5 checkpoints

Other Community Checkpoints: [here](https://huggingface.co/models?search=t5)

## Paper

For more information, please take a look at the original paper.

Paper: [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://arxiv.org/pdf/1910.10683.pdf)

Authors: *Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, Peter J. Liu* 


**Abstract**

Transfer learning, where a model is first pre-trained on a data-rich task before being fine-tuned on a downstream task, has emerged as a powerful technique in natural language processing (NLP). The effectiveness of transfer learning has given rise to a diversity of approaches, methodology, and practice. In this paper, we explore the landscape of transfer learning techniques for NLP by introducing a unified framework that converts every language problem into a text-to-text format. Our systematic study compares pre-training objectives, architectures, unlabeled datasets, transfer approaches, and other factors on dozens of language understanding tasks. By combining the insights from our exploration with scale and our new “Colossal Clean Crawled Corpus”, we achieve state-of-the-art results on many benchmarks covering summarization, question answering, text classification, and more. To facilitate future work on transfer learning for NLP, we release our dataset, pre-trained models, and code.

![model image](https://camo.githubusercontent.com/623b4dea0b653f2ad3f36c71ebfe749a677ac0a1/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f343030362f312a44304a31674e51663876727255704b657944387750412e706e67)

