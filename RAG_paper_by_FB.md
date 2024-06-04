# Retrieval-Augmented Generation for knowledge-intensive NLP tasks

Facebook Research [paper link](https://arxiv.org/pdf/2005.11401)

## Abstract
LLM problem: (based on 2021) 
1. Access and precisely manipulate knowledge is still limited. 
2. Updating knowledge is hard



RAG: 
- pre-trained parametric memory: pretrained seq2seq model 
[[RNN encoder-decoder paper](https://arxiv.org/pdf/1406.1078)] encoder:sequence to **c** / decoder: **c** to sequence
[[seq2seq](https://arxiv.org/pdf/1409.3215v3)]
- non-parametric memory: dense vector index of Wiki

Out performing NLP tasks:
- Open-domain QA
- Abstractive QA
- Jeopardy Question Generation
- Fact Verifation


## 1. Introduction

Pre-trained Neural Language Models: 
- Cannot easily expand or revise their memory
- May produce "Hallucianations"

Hybrid Models: Knowkedge can be derictly revised and expanded
- [REALM](https://arxiv.org/pdf/2002.08909) and [ORQA](https://arxiv.org/pdf/1906.00300) ==(What are they and their difference?)==
- FB AI research team bring the hybrid model to the "Workhorse of NLP" => Seq2seq model

General-purpose fune-tning approach -> RAG!!!

### RAG structure:
Retriver + Generator
![RAG_struc](./img/RAG_structure.png)
#### Retriever:
[Dense Passage Retriever](https://arxiv.org/pdf/2004.04906) ==(DPR)==
#### Generator:
- per output basis RAG-S
- per token basis RAG-T
### Tasks
knowledge-intensive tasks:
- NQ: open Natural Questions
- WQ: WebQuestions
- CT: CuratedTrec

Knowledge-intensive generation:
- MS-MARCO
- Jeopardy question

Fact Verification:
- FEVER
## 2. Methods


## 3. Experiments

## 4. Results

## 5. Related work

## 6. Discussion
