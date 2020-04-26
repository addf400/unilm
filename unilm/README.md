# UniLM
**Unified pre-training for language understanding (NLU) and generation (NLG)**

**UniLM v2** ```New``` (February, 2020): "[UniLMv2: Pseudo-Masked Language Models for Unified Language Model Pre-Training](https://arxiv.org/abs/2002.12804)".

**[UniLM v1](https://github.com/microsoft/unilm/tree/master/unilm-v1)** (September 30th, 2019): the code and pre-trained models for the NeurIPS 2019 paper entitled "[Unified Language Model Pre-training for Natural Language Understanding and Generation](https://arxiv.org/abs/1905.03197)".

### Abstractive Summarization - [Gigaword](https://github.com/harvardnlp/sent-summary)

The training set of Gigaword contains 3.8M examples for headline generation.

| Model                                                                            | ROUGE-1   | ROUGE-2   | ROUGE-L   |
| -------------------------------------------------------------------------------- | --------- | --------- | --------- |
| [OpenNMT](https://aclweb.org/anthology/P18-1015)                                 | 36.73     | 17.86     | 33.68     |
| [Re3Sum (Cao et al., 2018)](https://aclweb.org/anthology/P18-1015)               | 37.04     | 19.03     | 34.46     |
| [MASS (Song et al., 2019)](http://proceedings.mlr.press/v97/song19d/song19d.pdf) | 38.73     | 19.71     | 35.96     |
| [BertShare (Rothe et al., 2019)](https://arxiv.org/pdf/1907.12461.pdf)           | 38.13     | 19.81     | 35.62     |
| **UniLM**                                                                        | **38.90** | **20.05** | **36.00** |

### Abstractive Summarization - [CNN / Daily Mail](https://github.com/harvardnlp/sent-summary)

| Model                                                                                                                                                     | ROUGE-1   | ROUGE-2   | ROUGE-L   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- | --------- | --------- |
| [PGNet (See et al., 2017)](https://www.aclweb.org/anthology/P17-1099)                                                                                     | 39.53     | 17.28     | 36.38     |
| [Bottom-Up (Gehrmann et al., 2018)](https://www.aclweb.org/anthology/D18-1443)                                                                            | 41.22     | 18.68     | 38.34     |
| [GPT-2 TL;DR: (Radford et al., 2019)](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) | 29.34     | 8.27      | 26.58     |
| [MASS (Song et al., 2019)](https://github.com/microsoft/MASS#results-on-abstractive-summarization-9272019)                                                | 42.12     | 19.50     | 39.01     |
| [BertShare (Rothe et al., 2019)](https://arxiv.org/pdf/1907.12461.pdf)                                                                                    | 39.25     | 18.09     | 36.45     |
| [BertSumAbs (Liu and Lapata, 2019)](https://arxiv.org/pdf/1908.08345.pdf)                                                                                 | 41.72     | 19.39     | 38.76     |
| **UniLM**                                                                                                                                                 | **43.08** | **20.43** | **40.34** |

### Question Generation - [SQuAD](https://arxiv.org/abs/1806.03822)

We present the results following the same [data split](https://github.com/xinyadu/nqg/tree/master/data) and [evaluation scripts](https://github.com/xinyadu/nqg/tree/master/qgevalcap) as in [(Du et al., 2017)](https://arxiv.org/pdf/1705.00106.pdf).

| Model                                                              | BLEU-4    | METEOR    | ROUGE-L   |
| ------------------------------------------------------------------ | --------- | --------- | --------- |
| [(Du and Cardie, 2018)](https://www.aclweb.org/anthology/P18-1177) | 15.16     | 19.12     | -         |
| [(Zhang and Bansal, 2019)](https://arxiv.org/pdf/1909.06356.pdf)   | 18.37     | 22.65     | 46.68     |
| **UniLM**                                                          | **22.78** | **25.49** | **51.57** |

We also report the results following the data split as in [(Zhao et al., 2018)](https://aclweb.org/anthology/D18-1424), which uses the reversed dev-test setup.

| Model                                                            | BLEU-4    | METEOR    | ROUGE-L   |
| ---------------------------------------------------------------- | --------- | --------- | --------- |
| [(Zhao et al., 2018)](https://aclweb.org/anthology/D18-1424)     | 16.38     | 20.25     | 44.48     |
| [(Zhang and Bansal, 2019)](https://arxiv.org/pdf/1909.06356.pdf) | 20.76     | 24.20     | 48.91     |
| **UniLM**                                                        | **24.32** | **26.10** | **52.69** |

## Acknowledgments
Our code is based on [pytorch-transformers v0.4.0](https://github.com/huggingface/pytorch-transformers/tree/v0.4.0). We thank the authors for their wonderful open-source efforts.

## License
This project is licensed under the license found in the LICENSE file in the root directory of this source tree.
Portions of the source code are based on the [pytorch-transformers v0.4.0](https://github.com/huggingface/pytorch-transformers/tree/v0.4.0) project.

[Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct)

### Contact Information

For help or issues using UniLM, please submit a GitHub issue.

For other communications related to UniLM, please contact Li Dong (`lidong1@microsoft.com`), Furu Wei (`fuwei@microsoft.com`).

