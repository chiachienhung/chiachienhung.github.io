---
title: "**ZusammenQA: Data Augmentation with Specialized Models for Cross-lingual Open-retrieval Question Answering System**"
collection: publications
permalink: 
date: 2022-07-10
venue: 'Proceedings of the Workshop on Multilingual Information Access (MIA), NAACL'
 
---
**Chia-Chien Hung**, Tommaso Green, Robert Litschko, Tornike Tsereteli, Sotaro Takeshita, Marco Bombieri, Goran Glavaš, Simone Paolo Ponzetto
 [PDF](https://aclanthology.org/2022.mia-1.8.pdf) [CODE](https://github.com/umanlp/ZusammenQA)

This paper introduces our proposed system for the MIA Shared Task on Cross-lingual Openretrieval Question Answering (COQA). In this challenging scenario, given an input question the system has to gather evidence documents from a multilingual pool and generate from them an answer in the language of the question. We devised several approaches combining different model variants for three main components: Data Augmentation, Passage Retrieval, and Answer Generation. For passage retrieval, we evaluated the monolingual BM25 ranker against the ensemble of re-rankers based on multilingual pretrained language models (PLMs) and also variants of the shared task baseline, re-training it from scratch using a recently introduced contrastive loss that maintains a strong gradient signal throughout training by means of mixed negative samples. For answer generation, we focused on languageand domain-specialization by means of continued language model (LM) pretraining of existing multilingual encoders. Additionally, for both passage retrieval and answer generation, we augmented the training data provided by the task organizers with automatically generated question-answer pairs created from Wikipedia passages to mitigate the issue of data scarcity, particularly for the low-resource languages for which no training data were provided. Our results show that language- and domain-specialization as well as data augmentation help, especially for low-resource languages.