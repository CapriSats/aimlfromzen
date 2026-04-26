# Invento Robotics: Challenges in Building Enterprise Chatbots with LLMs: A Banking Case Study (2024)

https://medium.com/@balajivis/whats-so-challenging-about-building-chatbots-drawing-lessons-from-the-trenches-1ca7343c6e3d

## Short Summary

A bank's attempt to implement a customer support chatbot using GPT-4 and RAG reveals the complexities and challenges of deploying LLMs in production. What was initially estimated as a three-month project struggled to deliver after a year, highlighting key challenges in domain knowledge management, retrieval effectiveness, conversation flow design, state management, latency, and regulatory compliance.

## Long Summary

# Building Enterprise Chatbots with LLMs: Lessons from a Banking Implementation

## Overview

This case study examines a bank's journey in implementing a customer support chatbot using GPT-4 and modern LLM technologies. The implementation highlights the gap between theoretical simplicity and practical challenges in deploying LLMs in production environments. The study provides valuable insights into why even major tech companies struggle with full-scale chatbot deployments.

## Initial Approach and Assumptions

• Project started in early 2023 with high optimism following GPT-4's release
• Initial technical stack planned:
• Timeline estimation: 3 months for proof of concept
• Assumption of straightforward implementation due to available LLM capabilities
## Key Technical Challenges Encountered

### Domain Knowledge Management

• Complex knowledge distribution across multiple systems:
• Challenge of comprehensively capturing and structuring domain expertise
• Need for sophisticated knowledge extraction and organization systems
### Retrieval System Limitations

• RAG implementation proved more complex than anticipated
• Vector database challenges:
• Need for sophisticated retrieval optimization beyond basic similarity search
### Conversation Flow Architecture

• Complexity in designing natural conversation flows
• Challenges in balancing:
• Need for domain-specific conversation patterns
• Implementation of different conversation styles for various use cases
### State Management

• LLMs' stateless nature requiring additional architecture
• Multiple storage requirements:
• Complex memory management across conversation sessions
## Production Challenges

### Performance and Latency

• Multi-second delays affecting user experience
• Particular challenges in voice-based interactions
• Need for optimization strategies:
### Regulatory Compliance

• Financial sector-specific compliance requirements
• Need for:
### Response Control and Safety

• Challenge of preventing inappropriate promises or commitments
• Need for robust guardrails
• Balance between helpfulness and risk management
## Industry Context and Broader Implications

### Market Reality Check

• Even major tech companies (Amazon, Google, Microsoft) haven't fully implemented chatbots for critical support
• OpenAI's own experience:
• Demonstrates industry-wide challenges in production deployment
### Lessons Learned

• LLM implementation complexity often underestimated
• Need for comprehensive planning across:
• Importance of realistic timeline expectations
• Value of phased approach rather than full deployment
## Technical Requirements for Success

### Infrastructure Needs

• Robust vector database implementation
• Efficient knowledge graph architecture
• High-performance computing resources
• Low-latency storage solutions
### Process Requirements

• Comprehensive domain knowledge capture
• Sophisticated conversation flow design
• Regular model evaluation and updating
• Compliance monitoring systems
• Performance optimization protocols
## Best Practices Emerging

• Start with limited scope and expand gradually
• Implement strong monitoring and evaluation systems
• Build robust fallback mechanisms
• Maintain human oversight where needed
• Regular testing and validation of responses
• Continuous improvement of knowledge base
• Performance optimization as an ongoing process
## Conclusion

The case study reveals that successful LLM implementation in production, particularly for enterprise chatbots, requires significantly more infrastructure, planning, and ongoing maintenance than initially assumed. The experience highlights the importance of realistic expectations and comprehensive planning in LLMOps projects.


