# Wayfair: AI-Powered Co-pilot System for Digital Sales Agents (2024)

https://www.aboutwayfair.com/careers/tech-blog/agent-co-pilot-wayfairs-gen-ai-assistant-for-digital-sales-agents

## Short Summary

Wayfair developed an AI-powered Agent Co-pilot system to assist their digital sales agents during customer interactions. The system uses LLMs to provide contextually relevant chat response recommendations by considering product information, company policies, and conversation history. Initial test results showed a 10% reduction in handle time, improving customer service efficiency while maintaining quality interactions.

## Long Summary

# Wayfair's Agent Co-pilot: An LLM-Powered Sales Assistant System

## System Overview

Wayfair has developed an innovative AI-powered system called Agent Co-pilot to enhance their digital sales operations. Unlike traditional rule-based chatbots, this system works alongside human sales agents, providing real-time, contextually relevant chat response suggestions. The system is designed to help agents serve customers more efficiently while maintaining high-quality interactions.

## Technical Architecture and Implementation

### Prompt Engineering and Context Management

The system utilizes a sophisticated prompting strategy that incorporates multiple components:

• Task Description - Specific instructions for the LLM about the required action
• Guidelines - Internal rules and processes for customer interactions
• Policies - Current company policies on shipping, returns, and services
• Product Information - Relevant product data for specific customer inquiries
• Conversation History - Complete context of the ongoing customer interaction
### LLM Integration

• The system employs Large Language Models as its core technology
• Uses an iterative token generation process for response creation
• Implements probability-based token selection for generating contextually appropriate responses
• Allows agents to modify suggested responses for enhanced accuracy and personalization
## Quality Assurance and Monitoring

### Response Quality Metrics

The system implements comprehensive quality monitoring through various metrics:

• Prompt Instruction Adherence
• Factual Accuracy
• Edit Analysis
• Message Purpose Analysis
### Performance Metrics

The system tracks several key performance indicators:

• Average Handle Time (AHT)
• Order conversion rates
• Adoption rates at both contact and response levels
• Edit distance measurements
## Production Results and Impact

• Achieved 10% reduction in handle time
• Improved customer service efficiency
• Maintained high-quality customer interactions
• Identified areas for contextual enrichment
• Demonstrated positive impact on agent productivity
## Quality Assurance Implementation

The team employs a dual-approach quality assurance system:

• Utilizes both quantitative and qualitative data analysis
• Implements regular agent feedback reviews
• Analyzes conversation logs
• Employs a separate QA LLM for response quality assessment
• Maintains continuous system refinement processes
## Future Development Roadmap

### Retrieval Augmented Generation (RAG)

• Planning implementation of RAG techniques
• Will enable access to real-time Wayfair data
• Integration with product reviews database
• Enhanced policy and customer preference access
• Improved contextual understanding capabilities
### Model Fine-tuning Initiatives

• Development of specialized model training
• Focus on top-performing agent conversation styles
• Enhancement of tone and salesmanship
• Optimization for customer satisfaction
• Improved sales conversion potential
## Operational Considerations

### Data Integration

• Real-time product information access
• Policy database connectivity
• Customer interaction history integration
• Internal guidelines and process documentation
• Sales performance metrics
### System Monitoring

• Continuous performance tracking
• Regular quality assessments
• Response accuracy monitoring
• Agent adoption rate analysis
• Customer satisfaction metrics
### Deployment Strategy

• Gradual rollout approach
• Regular system updates
• Continuous feedback incorporation
• Performance optimization
• Agent training and support
The Agent Co-pilot system represents a sophisticated implementation of LLMs in a production environment, with careful attention to quality control, monitoring, and continuous improvement. The system's success is attributed to its comprehensive approach to context management, quality assurance, and performance monitoring, while maintaining focus on both agent efficiency and customer satisfaction.


