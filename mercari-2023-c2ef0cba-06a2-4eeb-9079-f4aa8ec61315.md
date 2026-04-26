# Mercari: Building AI Assist: LLM Integration for E-commerce Product Listings (2023)

https://engineering.mercari.com/en/blog/entry/20231219-leveraging-llms-in-production-looking-back-going-forward/

## Short Summary

Mercari developed an AI Assist feature to help sellers create better product listings using LLMs. They implemented a two-part system using GPT-4 for offline attribute extraction and GPT-3.5-turbo for real-time title suggestions, conducting both offline and online evaluations to ensure quality. The team focused on practical implementation challenges including prompt engineering, error handling, and addressing LLM output inconsistencies in a production environment.

## Long Summary

# Building AI Assist at Mercari: A Comprehensive LLMOps Case Study

Mercari, a major C2C marketplace platform, implemented an AI Assist feature to enhance seller experiences by leveraging Large Language Models (LLMs). This case study details their journey in implementing LLMs in production, highlighting key operational challenges and solutions.

# Team Structure and Approach

• Small, focused Generative AI/LLM team combining PMs, designers, and engineers
• Emphasis on close communication between roles for rapid iteration
• Dual focus on building products and enabling other teams to implement LLMs
• Regular technical experimentation to assess feasibility
• Continuous monitoring of field developments through social media, news, and research papers
# Technical Implementation Details

## Model Selection and Architecture

• Chose commercial APIs over open-source models
• Utilized GPT-4 and GPT-3.5-turbo for different aspects of the system
• Implemented a hybrid approach:
• Incorporated simple retrieval-augmented generation (RAG) techniques
• Focus on optimal user experience and sustainable LLM workflows
## Evaluation Framework

### Offline Evaluation

• Assessment of prompt effectiveness
• Focus on token usage optimization
• Quality assessment through manual review and automated evaluation
• Cost estimation for full-scale deployment
### Online Evaluation

• Partial release strategy for testing
• Real-time performance monitoring with user-generated content
• Initial simplified testing with binary responses
• Systematic tracking of response inconsistencies
## Production Challenges and Solutions

### Data Processing

• Implementation of robust pre-processing for user-generated content
• Post-processing logic to ensure consistent output format
• Special handling for language-specific token count variations
• Careful management of multilingual content (Japanese/English considerations)
### Error Handling

• Comprehensive API error management
• Integration with existing content moderation systems
• Token count optimization across different languages
### Quality Control Measures

• Continuous monitoring of model outputs
• Detection and handling of hallucinations
• Format consistency checks
• Performance optimization for high-traffic scenarios
# Operational Best Practices

## System Design Considerations

• Balance between cost and performance
• Modular architecture for easy updates
• Scalable infrastructure for handling varying loads
• Integration with existing marketplace systems
## Monitoring and Maintenance

• Regular performance assessment
• Cost tracking and optimization
• Content quality monitoring
• API usage tracking and optimization
## Future Development Plans

• Focus on LLM operations improvements
• Development of automated workflows
• Exploration of parameter-efficient fine-tuning
• Continuous experimentation with new techniques
# Key Learnings and Insights

## Technical Insights

• Importance of proper preprocessing and post-processing
• Need for robust error handling
• Value of gradual deployment strategy
• Significance of continuous evaluation
## Operational Insights

• Critical role of team communication
• Importance of domain expertise in ML/NLP
• Need for flexible architecture to accommodate rapid field changes
• Value of preliminary testing with simplified implementations
## Cost Management

• Strategic use of different models based on requirements
• Token usage optimization
• Language-specific cost considerations
• Balance between feature quality and operational costs
# Future Considerations

• Development of automated workflows
• Exploration of more complex specialized tasks
• Investigation of parameter-efficient fine-tuning
• Continuous adaptation to field developments
• Focus on operational efficiency improvements
• Regular reassessment of model selection based on evolving needs
# Mercari AI Assist: LLM Integration Case Study

## Overview

Mercari, a major e-commerce marketplace, implemented LLMs to enhance their platform's user experience through an AI Assist feature. The project focused on helping sellers create better product listings by providing intelligent suggestions for item titles and descriptions. This case study demonstrates a practical approach to integrating commercial LLMs into a production environment while addressing real-world challenges.

## Team Structure and Approach

• Small, focused Generative AI/LLM team with close collaboration between:
• Emphasis on constant communication to align expectations about LLM capabilities
• Regular technical experimentation for feasibility assessment
• Continuous monitoring of field developments through:
## Technical Implementation

### Model Selection and Architecture

• Strategic use of multiple OpenAI models:
• Two-part system design:
### Evaluation Framework

• Comprehensive dual evaluation approach:
### Production Challenges and Solutions

### Output Consistency Management

• Implemented rigorous pre-processing for user-generated content
• Developed post-processing logic for output format validation
• Handled various response format inconsistencies:
### Error Handling


