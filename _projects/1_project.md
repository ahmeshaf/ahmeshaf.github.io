---
layout: page
title: Event coreference resolution with GPT
description: Possible course project for incoming students to explore
img: assets/img/projects/coref_1.jpg
importance: 1
category: "nlp-course-project"
---

## Introduction

Event coreference resolution (ECR) is the task of finding mentions of the same event within 
the same document (known as *within-document coreference resolution*, or WDCR), or across 
text (known as *cross-document coreference resolution*, or  CDCR) documents. 
This task is used for knowledge graph construction, event salience detection and question answering.

Consider the following examples with marked event triggers (word or phrase referring to the event):


<style>
  ol {
    counter-reset: custom-counter;

  }

  nli {
    list-style: none;
    counter-increment: custom-counter;
  }

  nli::before {
    content: "E" counter(custom-counter) ":";
    font-weight: bold;
    margin-right: 5px;
  }
</style>

<ol>
  <nli>55-year-old star will <b><i>replace</i></b> Matt Smith, who announced in June that he was leaving the sci-fi show.</nli>
<br/>
<nli>Matt Smith, 26, will make his debut in 2010, <b><i>replacing</i></b> David Tennant, who leaves at the end of this year.</nli>
<br/>
<nli>Peter Capaldi <b><i>stepped into</i></b> Matt Smith's soon to be vacant Doctor Who shoes.</nli>

</ol>

Now the task of ECR is to predict that E1 and E3 are coreferring events, and that E2 is a related but 
different event from E1 and E3.

ECR is typically tackled by performing pairwise predictions on mention pairs, then, clustering on
those predictions. The pairwise scorer is trained by using a joint feature space of the two mentions.
Now, the goal of this project is to probe GPT-4 by using it as the pairwise scorer. The task involves 
engineering various strategies for in-context learning.
## Motivation
## References
 - [https://aclanthology.org/2023.findings-acl.100](https://aclanthology.org/2021.emnlp-main.106/)
 - [https://aclanthology.org/2021.emnlp-main.106/](https://aclanthology.org/2021.emnlp-main.106/)

## GitHub Repo
[https://github.com/ahmeshaf/lemma_ce_coref](https://github.com/ahmeshaf/lemma_ce_coref)

You can fork this repository for this project
## Required Skills
1. pyhon experience with PyTorch, Huggingface, OpenAI GPT API, spaCy
2. writing: LateX
3. git: Ability to collaborate and maintain a code repository

## Deadlines
A. November 15, 2023

B. December 15, 2023
