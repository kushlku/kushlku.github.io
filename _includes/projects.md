## Projects
### End-to-End GenAI Entity Resolution Workflow, _2024-present_
Developed a scalable pay-as-you-go entity resolution workflow that integrates representation learning, entity matching, 
and generative AI to improve product variation curation and correction. Key innovations include: (1) applying non-parametric 
clustering as a lossless alternative to blocking to scale pairwise matching, (2) performant distilled multi-modal
LLM matcher model to obtain curated cluster merge probabilities, (3) highly efficient off-the-shelf LLM inference for 
cluster deduplication, and (4) graph-pruning to surface most informative and uncertain edges in a cluster-cluster graph 
for human evaluation. The new workflow was provably more efficient and achieved _99%_ precision and at least _90%_ recall 
with more than _5X_ reduction in human touchpoint. 

### Scalable Product Retrieval and Blocking Service, _2023-2024_
Built a scalable product retrieval service using multi-modal CLIP-like models trained in a distributed setup. 
Optimized for large-batch contrastive learning, the models demonstrated strong generalizability across product 
types and product relationships, enabling task-agnostic retrieval and blocking for large-scale pairwise workflows. 
The service significantly outperformed baselines such as token-overlap based blocking system and enabled _95%_ recall
and efficient product retrieval using multi-modal representations and approximate nearest neighbor search optimizations.
This work led to CIKM'24 publication titled [Unsupervised Multi-Modal Representation Learning for High Quality 
Retrieval of Similar Products at E-commerce Scale](https://dl.acm.org/doi/pdf/10.1145/3583780.3615504) as an oral paper.


### Multi-Attribute Entity Extraction using Transformers, _2021-2022_
Extended Convolutional Neural Network (CNN) based single-attribute entity extraction to multi-attribute entity
extraction using Transformers architecture that were more performant. This reduced the need to maintain separate models per 
product attribute and locale, creating an operationally efficient model-building pipeline and faster goal delivery.
Moreover, transformer extraction models exhibited better context awareness for more accurate entity prediction based on
correlation to other entities, even when certain entity values were missing or noisy.
