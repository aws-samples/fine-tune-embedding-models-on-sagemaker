## Fine-Tuning Embedding Models on SageMaker

This repository contains samples for fine-tuning embedding models using Amazon SageMaker. Embedding models are useful for tasks such as semantic similarity, text clustering, and information retrieval.  
By fine-tuning embedding model on data that is representative of the target domain or task, the model can learn to capture the relevant semantics, jargon, and contextual relationships that are crucial for that domain.  
Domain-specific embeddings can significantly improve the quality of vector representations, leading to more accurate retrieval of relevant context from the vector database. This, in turn, enhances the performance of the RAG system in terms of generating more accurate and relevant responses.


## Contents
- `sentence-transformer/`: This directory contains a Jupyter notebook demonstrating how to fine-tune a sentence embedding model using the Multiple Negatives Ranking Loss technique. The Multiple Negatives Ranking Loss function is recommended when in your training data you only have positive pairs, for example, only pairs of similar texts like pairs of paraphrases, pairs of duplicate questions, pairs of (query, response), or pairs of (source_language, target_language).
We are using the Multiple Negatives Ranking Loss function because we are utilizing Bedrock FAQ as the training data, which consists of pairs of questions and answers.  
The code in this directory is used in the AWS blog post "Improve RAG accuracy with finetuned embedding models on Sagemaker"
  
## Security
We welcome contributions from the community! If you have an example or sample for fine-tuning embedding models on SageMaker, please feel free to submit a pull request. Your contribution will help others in their journey of fine-tuning embedding models.  

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

