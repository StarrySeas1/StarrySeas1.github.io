---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

# Recent Projects

## Large Language Model

&emsp;&emsp; YuxinGPT is an autoregressive language model trained on a 189GB Chinese corpus with parameters of 220M/1B/3B/13B. Due to its main focus on the domains of psychology and astrology, we increased the proportion of data related to psychology and astrology compared to other general domain models (LLaMA, BLOOM). This specialization enables YuxinGPT to excel in downstream tasks related to these two domains. In our evaluation, YuxinGPT outperforms the fine-tuned LLaMA-7B and BLOOM-7B1 models and slightly underperforms ChatGLM-6B on our constructed test set.

![Fig.1](/images/WX20230614-171632.png){:height="50%" width="50%"}

Case study

![Fig.2](/images/YxGPT_01.jpg){:height="60%" width="60%"}

![Fig.3](/images/YxGPT_02.jpg){:height="60%" width="60%"}

## Large Language Model(mT5-Large-770M) for solving applied math problems in primary and secondary schools.

&emsp;&emsp; In order to enhance support for downstream tasks and address automated mathematical problem-solving through a seq2seq model, we have developed Math-LLM. This model has been trained for a duration of two weeks using a T5 architecture on two TPUs, leveraging a parallel corpus of over 2 million instances. Extensive testing across multiple downstream tasks has revealed that Math-LLM exhibits the ability to generate accurate problem-solving approaches. While occasional errors in specific numerical values may occur, Math-LLM demonstrates remarkable performance in tasks such as generating explanatory content and effectively classifying problem types.

![Fig.7](/images/math-llm.png){:height="50%" width="50%"}


## Knowledge-based conversational system using large-scale language model
&emsp;&emsp; Large-scale language models perform well on text generation tasks, but they often suffer from hallucination problems, especially in knowledge-based question answering. To solve this problem, we introduce a knowledge graph and search engine, and format the input of the model into a conversational format. In our evaluation, this improvement significantly reduces the search space of text generation models by analyzing user input through NER, knowledge graphs and search engines, constructing prompts containing knowledge, and then inputting spliced ​​prompt text into the model, thus alleviating the impact of the hallucination problem on the generated text.

![Fig.4](/images/KBChatBot.png){:height="50%" width="50%"}

<!-- Demo: 192.168.1.1 -->

## Hierarchical text generation based on block-masked MT5.

&emsp;&emsp; When solving a math problem, a qualified teacher will often divide the entire problem-solving process into several parts to facilitate students' understanding of the problem. The figure below illustrates the different explanatory texts corresponding to different parsing steps.
![Fig.5](/images/Explain_the_interpretation_of_the_segment.png)
In the process of explaining a complete problem-solving procedure, it needs to be explained in several small parts. We control the generation of explanatory text at different levels by setting different attention mask matrices. Because the parsing steps of the MWP are organized in a tree structure, the parsing text fragment corresponding to the parent node and the parsing text fragment corresponding to the child node partially overlap. When constructing a parallel corpus, the source text is not very different, but the target text is different. Due to the existence of repeated segments, if the parent node and the child node are regarded as an independent sample, the proportion of the child node in the training set is increased implicitly, thus affecting the generation of the overview text of the parent node. In order to solve this problem, the tree structure text features are extracted by modifying the form of the Attention Mask matrix.
![Fig.6](/images/attention_mask.png)

## Combining Image and Text for Chinese Spelling Correction

&emsp;&emsp; Correcting spelling mistakes is a complex task that presents significant challenges in obtaining satisfactory solutions. In this study, we focus on Chinese spelling error correction (CSC). The state-of-the-art method utilizes the BERT architecture to detect and correct errors in a single sentence, and the joint training of error detection and error correction effectively reduces cascading errors. However, deploying such models in real-world scenarios often encounters false and missed corrections due to OCR errors. To address this issue, we propose an innovative approach to combine image and text information, exploiting visual cues to improve the performance of the entire error correction pipeline in scenarios where OCR is inaccurate. Our evaluation demonstrates the potential of this approach in real-world scenarios to address both miscorrections and missed corrections, leading to more precise and comprehensive error detection and correction. [Paper](/files/paper_01.pdf)

<!-- ## College entrance examination (CEE) math problem-solving robot.

blabla -->

<!-- # [Research](https://www.researchgate.net/scientific-contributions/Shitong-Qin-2119476520) -->
# Research

## Journal Papers:

Shitong Qin, Leqi Sha, et al. Combining Image and Text for Chinese Spelling Correction. DOI: 10.13140/RG.2.2.34400.87046. [Paper](https://www.researchgate.net/publication/371684241_Combining_Image_and_Text_for_Chinese_Spelling_Correction)

------

The following papers are published in the field of electronic information

------

Qin, Shitong & Renxian, Li & Yang, Ruiping & Ding, Chunying. (2016). Debye series analysis of internal and near-surface fields for a homogeneous sphere illuminated by an axicon-generated vector Bessel beam. Journal of Quantitative Spectroscopy and Radiative Transfer. 195. 10.1016/j.jqsrt.2016.12.025. [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0022407316304861)

Yang, Ruiping & Renxian, Li & Qin, Shitong & Ding, Chunying & Mitri, F. (2017). Direction reversal of the optical spin torque on a Rayleigh absorptive sphere in vector Bessel polarized beams. Journal of Optics. 19. 025602. 10.1088/2040-8986/19/2/025602. [Paper](https://iopscience.iop.org/article/10.1088/2040-8986/19/2/025602)

Wen, Yao & Xi, Qiangli & Renxian, Li & Qin, Shitong & Ding, Chunying. (2017). Scattering of a vector Bessel-Gaussian beam by a sphere. Journal of Quantitative Spectroscopy and Radiative Transfer. 204. 10.1016/j.jqsrt.2017.08.025. [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0022407317303953)

Wen Y, Xi Q, Li R, et al. Scattering of a vector Bessel-Gaussian beam by a sphere[J]. Journal of Quantitative Spectroscopy and Radiative Transfer, 2018, 204: 165-178. [Paper](https://www.sciencedirect.com/science/article/abs/pii/S0022407317303953)

Yang R, Li R, Qin S, et al. Direction reversal of the optical spin torque on a Rayleigh absorptive sphere in vector Bessel polarized beams[J]. Journal of Optics, 2016, 19(2): 025602. [Paper](https://iopscience.iop.org/article/10.1088/2040-8986/19/2/025602)
