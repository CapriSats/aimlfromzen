# Various: Panel Discussion on Building Production LLM Applications (2023)

https://www.youtube.com/watch?v=usF1Q7tzJD0

## Short Summary

A panel discussion featuring experts from Various companies discussing key aspects of building production LLM applications. The discussion covers critical topics including hallucination management, prompt engineering, evaluation frameworks, cost considerations, and model selection. Panelists share practical experiences and insights on deploying LLMs in production, highlighting the importance of continuous feedback loops, evaluation metrics, and the trade-offs between open source and commercial LLMs.

## Long Summary

# Panel Discussion on Production LLM Applications: Key Insights and Best Practices

## Overview

This panel discussion brought together experts from various companies and backgrounds to discuss practical aspects of building and deploying LLM applications in production. The panelists included Smitha from PromptOps, George Matthew from Insight Partners, Natalia Barina from Meta, and Sahar Moore from Stripe, with Sam Charrington moderating.

## Key Perspectives on LLMs

### Hallucinations and Model Capabilities

• Panelists argued that hallucinations might be a permanent feature rather than a bug
• Focus should be on finding appropriate use cases rather than eliminating hallucinations entirely
• Strong emphasis on open source models as the future of LLM deployments
• Trend toward domain-specific specialized models leveraging proprietary data
## Framework for LLM Use Case Selection

### Evaluation Axes

• Fluency vs. Accuracy trade-off framework for assessing use cases
• Business decision framework considering factors like:
### Practical Implementation Tips

### Prompt Engineering Best Practices

• Use structured outputs (JSON, markdown)
• Include examples and relevant context
• Leverage vector databases for semantic similarity search
• Implement prompt chaining for complex tasks
• Add citations to reduce hallucinations
• Use role-based prompting
### Latency Management

• Implement streaming responses
• Split prompts into multiple steps
• Show intermediate results to users
• Use UX features to mask latency
## Evaluation and Quality Control

### Testing Approaches

• Automated evaluation using superior models (e.g., GPT-4 to evaluate GPT-3.5)
• Benchmark questions spanning multiple areas
• Semantic similarity scoring
• Keyword-based evaluation
• Regular testing frequency
### Feedback Loops

• Continuous improvement through user feedback
• Integration of reinforcement learning with human feedback (RLHF)
• Version control for prompts
• Regular benchmark updates
## Cost Optimization Strategies

### Economic Considerations

• Balance between prompt detail and inference costs
• Trade-offs between model size and performance
• Strategic use of caching mechanisms
• Consideration of fine-tuning vs. prompt engineering
### Model Selection Framework

• Start with powerful models (e.g., GPT-4) for initial testing
• Consider downgrading to more cost-effective options after validation
• Evaluate open source alternatives
• Consider multi-model approaches for different requirements
## Production Deployment Considerations

### Risk Management

• Implementation of AI System Cards for transparency
• Comprehensive evaluation of safety risks
• Regular monitoring and assessment
• Clear documentation of model limitations
### Technical Infrastructure

• Vector database integration
• Prompt versioning systems
• Evaluation frameworks
• Feedback collection mechanisms
## Future Trends and Recommendations

### Emerging Patterns

• Movement toward smaller, specialized models
• Increasing importance of private data
• Growth of open source alternatives
• Evolution of evaluation frameworks
### Best Practices for Teams

• Start with extensive experimentation
• Build robust evaluation frameworks
• Implement continuous feedback loops
• Consider both open source and commercial options
• Focus on use case appropriateness
• Maintain flexibility in model selection
## Implementation Challenges

### Common Issues

• Lack of standardized evaluation frameworks
• Balancing cost with performance
• Managing latency in production
• Handling model updates and versions
• Integrating feedback effectively
### Solutions and Mitigations

• Use of model blending techniques
• Implementation of robust testing frameworks
• Regular performance monitoring
• Continuous collection of user feedback
• Strategic use of caching and optimization techniques
The discussion emphasizes the practical aspects of deploying LLMs in production, highlighting the importance of careful evaluation, continuous improvement, and appropriate use case selection. The panelists stress that success in LLM deployment comes from understanding both the technical capabilities and limitations while building robust frameworks for evaluation and improvement.


