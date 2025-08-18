
### End-to-End Product Variations Workflow with GenAI
Developed a scalable pay-as-you-go auditing workflow that integrates representation learning, product matching, and 
generative AI to improve product variation curation and correction. Key innovations included: (1) applying density 
clustering as a practical alternative to micro-clustering to scale pairwise matching, and (2) leveraging 
graph-pruning techniques to filter out least informative cluster-to-cluster decisions.

| Timeline  | Tools                     | Models                     |
|-----------|---------------------------|----------------------------|
| 2024–2025 | AWS SageMaker, AWS EMR, PySpark | CLIP, QWEN2.5-3B, Claude Sonnet 4 |


### Scalable Product Retrieval Service
Built a scalable product retrieval service using multi-modal CLIP-like models trained in a distributed setup. 
Optimized for large-batch contrastive learning, the models demonstrated strong generalizability across product 
relationships, enabling task-agnostic blocking for large-scale pairwise workflows. The service significantly 
outperformed the existing token-overlap based blocking system.

| Timeline   | Tools                        |
|------------|------------------------------|
| 2022–2023  | AWS OpenSearch, PyTorch Distributed |


### Multi-Attribute Entity Extraction using Transformers
Extended Convolutional Neural Network (CNN) based single-attribute entity extraction to multi-attribute entity
extraction using more capacity transformer architecture. This reduced the need to maintain separate models per 
product attribute and locale, creating an operationally efficient model-building pipeline and faster goal delivery. 

| Timeline  | Libraries            |
|-----------|----------------------|
| 2021–2022 | HuggingFace, Pytorch |