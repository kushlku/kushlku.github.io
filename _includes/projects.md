## Projects
### Demeter: End-to-End GenAI Entity Resolution Workflow, _2024-present_
Developed a scalable pay-as-you-go entity resolution workflow for products that integrates representation learning, entity matching, 
and generative AI to improve de-duplication pipeline. Key innovations include: (1) applying nonparametric 
clustering as a lossless alternative to blocking to scale pairwise matching by cluster merging; (2) developing a performant, 
multimodal distilled LLM matcher to estimate match probabilities; (3) leveraging efficient off-the-shelf LLM inference for 
cluster canonicalization; and (4) pruning the cluster–cluster graph to obtain the most informative edges for human feedback. 
The new workflow was provably more efficient and achieved _99%_ precision and at least _90%_ recall with more than _5&times;_ 
reduction in human touchpoint.

### Mergen: Scalable Product Retrieval and Blocking Service, _2023-2024_
Built a scalable product retrieval service using multimodal CLIP-like models trained in a distributed setup. Optimized 
for large-batch training and efficient image loading, the models exhibited strong generalization across diverse product 
categories and product relationships, enabling task-agnostic retrieval and blocking for large-scale pairwise workflows. 
The service significantly outperformed baselines such as token-overlap based blocking system and achieved _95%_ recall
at _18%_ better reduction ratio with multimodal retrieval capabilities and _73%_ cheaper search. This work led to CIKM'24
publication titled [Unsupervised Multimodal Representation Learning for High Quality Retrieval of Similar Products at 
E-commerce Scale](https://dl.acm.org/doi/pdf/10.1145/3583780.3615504) as an oral paper.

### PAVE: Improve Recall of Product Attribute Extraction Models using Reinforcement Learning, _2022-2023_
Product attribute extraction models often suffer from low recall when product data has missing or noisy information. In
this project, we developed a Reinforcement Learning based method to improve recall of any product attribute extraction
model by leveraging information from neighbors of the given product. We formulated this problem as a first order Markov 
Decision Process and trained a Reinforcement Learning agent using Proximal Policy Optimization (PPO) using novel rewards 
to predict agent actions to choose the best attribute value from a ranked list of product neighbors. We show that our 
method outperforms several baselines to yield 10\% higher recall at same precision without needing larger context window
than the initial context window of the extraction model. This work was published in CIKM'22 titled 
[PAVE: Lazy-MDP based Ensemble to Improve Recall of Product Attribute Extraction Models](https://dl.acm.org/doi/pdf/10.1145/3511808.3557119) 
as an oral paper.


### Multi-Attribute Extraction using Transformers, _2021-2022_
Extended Convolutional Neural Network (CNN) based single-attribute entity extraction to multi-attribute entity
extraction using a Transformer-based architecture that was more performant. This reduced the need to maintain separate 
models per product attribute and locale, creating an operationally efficient model-building pipeline and faster goal delivery.
Moreover, Self-attention exhibited better context awareness for accurate multi-attribute extraction based on attribute 
relationships, for example knowledge of product type being a candy increases probability of 'orange' being a flavor
attribute than color. Such relational priors proved critical when attributes share overlapping domains.

### Modeling Price-Per-Unit for Consumables Products, _2020-2021_ 
Price-per-unit information is a crucial factor in purchase decision, especially in consumables products like grocery
and beauty products. In this project, we developed a scalable lightweight model to predict price per unit of products
at scale using its textual attributes like title and description as well as categorical information from product 
taxonomy. We formulated fact extraction as a two-step question answering problem to first predict type of quantity, like
weight, volume or count and then extract all the relevant quantity information using multi-span architecture. We show
that our method outperforms the state-of-the-art approaches like BERT while being lightweight and scalable. This work was
published in KDD 2021 Truefact Workshop titled [Solving Price Per Unit Problem Around the World: Formulating Fact
Extraction as Question Answering](https://arxiv.org/pdf/2204.05555).