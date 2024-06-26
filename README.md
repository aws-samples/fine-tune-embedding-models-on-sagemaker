## Fine-Tuning Embedding Models on SageMaker

This repository contains samples for fine-tuning embedding models using Amazon SageMaker. Embedding models are useful for tasks such as semantic similarity, text clustering, and information retrieval.  Fine-tuning these models on your specific domain data can greatly improve their performance.

## Contents
- `sentence-transformer/`: This directory contains a Jupyter notebook demonstrating how to fine-tune a sentence embedding model using the Multiple Negatives Ranking Loss technique. The Multiple Negatives Ranking Loss function is recommended when in your training data you only have positive pairs, for example, only pairs of similar texts like pairs of paraphrases, pairs of duplicate questions, pairs of (query, response), or pairs of (source_language, target_language).
We are using the Multiple Negatives Ranking Loss function because we are utilizing Bedrock FAQ as the training data, which consists of pairs of questions and answers.
  
## Security
We welcome contributions from the community! If you have an example or sample for fine-tuning embedding models on SageMaker, please feel free to submit a pull request. Your contribution will help others in their journey of fine-tuning embedding models.  

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

