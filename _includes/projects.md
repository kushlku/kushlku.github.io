## Projects
### End-to-End Product Variations Workflow with GenAI, 2024-present
Developed a scalable pay-as-you-go entity resolution workflow that integrates representation learning, entity matching, 
and generative AI to improve product variation curation and correction. Key innovations include: (1) applying density 
clustering as a lossless alternative to blocking to scale pairwise matching, (2) highly performant distilled multi-modal
LLM matcher model to avoid expensive off-the-shelf LLM inference, (3) efficient off-the-shelf LLM inference for 
efficient cluster deduplication, and (4) leveraging graph-pruning techniques to filter out least informative 
cluster-to-cluster decisions. The new workflow was provably more efficient and effective in achieving 99% precision and 
at least 90% recall with more than 5X reduction in human touchpoint. 

### Scalable Product Retrieval Service
Built a scalable product retrieval service using multi-modal CLIP-like models trained in a distributed setup. 
Optimized for large-batch contrastive learning, the models demonstrated strong generalizability across product 
relationships, enabling task-agnostic blocking for large-scale pairwise workflows. The service significantly 
outperformed the existing token-overlap based blocking system.


### Multi-Attribute Entity Extraction using Transformers
Extended Convolutional Neural Network (CNN) based single-attribute entity extraction to multi-attribute entity
extraction using more capacity transformer architecture. This reduced the need to maintain separate models per 
product attribute and locale, creating an operationally efficient model-building pipeline and faster goal delivery.
