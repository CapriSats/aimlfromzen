# Walmart: Hybrid AI System for Large-Scale Product Categorization (2024)

https://medium.com/walmartglobaltech/using-predictive-and-gen-ai-to-improve-product-categorization-at-walmart-dc9821c6a481

## Short Summary

Walmart developed Ghotok, an innovative AI system that combines predictive and generative AI to improve product categorization across their digital platforms. The system addresses the challenge of accurately mapping relationships between product categories and types across 400 million SKUs. Using an ensemble approach with both predictive and generative AI models, along with sophisticated caching and deployment strategies, Ghotok successfully reduces false positives and improves the efficiency of product categorization while maintaining fast response times in production.

## Long Summary

# Walmart's Ghotok: A Hybrid AI System for E-commerce Product Categorization

## Overview

Walmart developed a sophisticated AI system called Ghotok to handle the complex task of product categorization across their vast digital platform. With over 400 million SKUs, the system needed to efficiently organize products while maintaining a seamless shopping experience similar to their physical stores.

## Technical Architecture and Implementation

### Hybrid AI Approach

• Combines both Predictive AI and Generative AI in an ensemble model architecture
• Uses domain-specific features for training predictive models
• Leverages chain-of-thought prompting for generative AI components
• Implements a two-stage filtering process to reduce computational costs:
### Production Infrastructure

• Implements a two-tier caching system with LRU mechanism
• Optimized for handling millions of category-product type mappings
• Designed to meet millisecond-level service agreements
### Model Training and Optimization

### Predictive AI Components

• Trained on domain-specific features
• Hyperparameter optimization based on human-labeled datasets
• Multiple evaluation metrics:
### Generative AI Components

• No specific training on domain features required
• Utilizes pre-trained knowledge through chain-of-thought prompting
• Implements symbol tuning for improved performance
### Production Deployment Considerations

### Performance Optimization

• Two-stage filtering process to reduce computational load:
• Caching strategy implementation for fast access to frequently used mappings
### Exception Handling and Monitoring

• Dedicated exception handling tool combining ML and human intervention
• System designed to handle edge cases in production
• Quick resolution path for unexpected scenarios
## Key LLMOps Learnings and Best Practices

### Prompt Engineering

• Chain-of-thought reasoning proved crucial for improved model adherence
• Implementation of logical sequencing in prompts
• Focus on contextual relevance and logical consistency
### Model Optimization

• Symbol tuning techniques for improved performance
• Path representation optimization
• Careful balancing of model weights in ensemble
### Hallucination Management

• Strategic use of generative AI's semantic comprehension
• Leveraging billion-parameter models to validate million-parameter model outputs
• Cross-validation between predictive and generative components
### Production Monitoring and Maintenance

• Regular evaluation of false positive rates
• Implementation of quick resolution paths for edge cases
• Combination of automated and human oversight
## Technical Challenges and Solutions

### Scalability

• Handling millions of category-product type pairs
• Efficient storage and retrieval systems
• Optimized caching mechanisms
### Performance

• Meeting millisecond-level response requirements
• Balancing accuracy with speed
• Efficient resource utilization
### Quality Control

• Reduction of false positives
• Management of AI hallucinations
• Handling of edge cases
## Results and Impact

• Successful reduction in false positive rates
• Improved product categorization accuracy
• Enhanced customer experience through better product organization
• Efficient handling of 400 million SKUs
• Maintained fast response times in production environment
## Future Considerations

• Continuous optimization of model performance
• Regular updates to handle new product categories
• Ongoing refinement of exception handling processes
• Potential expansion to handle increasing product catalog

