
### End-to-End Product Variations Workflow with GenAI | 2024-2025
Developed a scalable pay-as-you-go auditing workflow that integrates representation learning, product matching, and 
generative AI to improve product variation curation and correction. Key innovations included: (1) applying density 
clustering as a practical alternative to micro-clustering to scale pairwise matching, and (2) leveraging 
graph-pruning techniques to filter out least informative cluster-to-cluster decisions.
**Tools:** AWS Sagemaker, AWS EMR, Pyspark | **Models:** CLIP, QWEN2.5-3B, CLaude Sonnet 4

### Scalable Product Retrieval Service | 2022-2023
Built a scalable product retrieval service using multi-modal CLIP-like models trained in a distributed setup. 
Optimized for large-batch contrastive learning, the models demonstrated strong generalizability across product 
relationships, enabling task-agnostic blocking for large-scale pairwise workflows. The service significantly 
outperformed the existing token-overlap based blocking system.
**Tools:** AWS OpenSearch, Pytorch Distributed
