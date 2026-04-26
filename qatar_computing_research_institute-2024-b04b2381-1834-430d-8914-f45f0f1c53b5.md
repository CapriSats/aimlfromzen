# Qatar Computing Research Institute: T-RAG: Tree-Based RAG Architecture for Question Answering Over Organizational Documents (2024)

https://arxiv.org/html/2402.07483v2

## Short Summary

Qatar Computing Research Institute developed a novel question-answering system for organizational documents combining RAG, finetuning, and a tree-based entity structure. The system, called T-RAG, handles confidential documents on-premise using open source LLMs and achieves 73% accuracy on test questions, outperforming baseline approaches while maintaining robust entity tracking through a custom tree structure.

## Long Summary

# Tree-Based RAG Architecture for Enterprise Document QA

This case study from Qatar Computing Research Institute (QCRI) describes the development and deployment of T-RAG, a novel question-answering system designed to handle confidential organizational documents. The system represents a comprehensive approach to building production LLM applications, combining multiple techniques while carefully considering real-world constraints and requirements.

## Core Problem and Requirements

The key challenge was building a QA system for confidential organizational documents that could:

• Run fully on-premise due to data security requirements
• Operate with limited computational resources
• Provide robust and accurate responses
• Handle complex entity relationships within organizational hierarchies
## Technical Architecture

The T-RAG system combines three key components:

### Base RAG Implementation

• Uses Chroma DB for vector storage
• Employs Maximum Marginal Relevance (MMR) for diverse document retrieval
• Utilizes the Instructor embedding model for text embeddings
• Implements standard RAG retrieval and generation pipeline
### Model Finetuning

• Uses Llama-2 7B as the base model
• Implements Parameter-Efficient Fine-Tuning (PEFT) via QLoRA
• Training dataset of 1,614 QA pairs generated from documents
• 90/10 train/validation split
• Achieved with only 33.5M trainable parameters (200x reduction)
• QLoRA enables 4-bit quantization for memory efficiency
### Tree-Based Entity Structure

• Custom tree representation of organizational hierarchy
• Integrated with spaCy for entity detection
• Generates textual context from tree traversal
• Augments standard RAG context with entity relationships
• Helps prevent entity-related hallucinations
## Development Process

The team followed a systematic approach to building the system:

### Data Preparation

• Manual conversion of tables to text
• Document chunking based on section headers
• Multi-stage QA pair generation:
• Quality checks and duplicate removal
### Implementation Choices

• On-premise deployment requirement led to open source model selection
• Limited compute guided choice of 7B parameter model
• Testing revealed benefits of combining approaches vs single method
### Evaluation Strategy

• Multiple rounds of user testing
• Custom evaluation metrics including "Correct-Verbose"
• Needle in a haystack tests for retrieval robustness
• MMLU testing to check for catastrophic forgetting
## Results and Performance

The system achieved meaningful improvements over baselines:

• Overall accuracy of 73% vs 56.8% for basic RAG
• Particularly strong on entity-related queries (100% on simple entity questions)
• Maintained robustness in needle-in-haystack tests
• Avoided major degradation of base model capabilities
## Key Lessons and Best Practices

The team documented several important insights for production LLM systems:

### Architecture Design

• Hybrid approaches combining multiple techniques often work best
• Tree structures can effectively represent hierarchical data
• Careful attention needed for context window management
• Entity handling requires special consideration
### Development Process

• Domain expert involvement is crucial
• Iterative testing with end users provides vital feedback
• Question phrasing sensitivity requires attention
• Careful evaluation of tradeoffs between approaches needed
### Model Training

• Finetuning requires careful monitoring for degradation
• PEFT techniques enable efficient adaptation
• Generated training data needs quality control
• System prompts require careful crafting
### Production Considerations

• Document update strategies must be planned
• Context retrieval optimization is crucial
• System needs to handle diverse query types
• Response verbosity requires management
## Monitoring and Maintenance

The system includes several key monitoring aspects:

• Tracking of correct vs verbose responses
• Entity detection accuracy monitoring
• Context retrieval effectiveness measures
• Model performance degradation checks
## Future Development

The team identified several areas for future work:

• Expansion to wider document corpus
• Development of chat-based interface
• Enhanced conversation history handling
• Improved context management strategies
## Technical Infrastructure

The implementation required specific infrastructure choices:

• 4 Quadro RTX 6000 GPUs (24GB each) for training
• Chroma DB for vector storage
• spaCy for entity detection
• Custom tree data structures
• Hugging Face PEFT library integration
This case study demonstrates a thoughtful approach to building production LLM systems that carefully balances various constraints while achieving robust performance. The combination of multiple techniques and careful attention to evaluation and monitoring provides valuable insights for similar enterprise deployments.


