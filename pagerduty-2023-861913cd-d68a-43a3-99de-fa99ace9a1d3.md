# PagerDuty: Rapid Development and Deployment of Enterprise LLM Features Through Centralized LLM Service Architecture (2023)

https://www.youtube.com/watch?v=ptqJ4prSHiA

## Short Summary

PagerDuty successfully developed and deployed multiple GenAI features in just two months by implementing a centralized LLM API service architecture. They created AI-powered features including runbook generation, status updates, postmortem reports, and an AI assistant, while addressing challenges of rapid development with new technology. Their solution included establishing clear processes, role definitions, and a centralized LLM service with robust security, monitoring, and evaluation frameworks.

## Long Summary

# PagerDuty's Journey to Production LLM Features

## Company Background and Challenge

PagerDuty, a SaaS platform for incident management and IT operations, embarked on an ambitious journey to integrate LLM capabilities into their product suite. Following the release of ChatGPT in late 2022, they set an aggressive goal to develop and deploy GenAI features within just two months, adopting a "think days not weeks" approach.

## GenAI Features Implemented

### Initial Release (Summer 2023)

• AI-generated runbooks - Allows users to describe desired automation scripts in natural language, generating appropriate runbook jobs
### September 2023 Releases

• Status Updates - AI-powered drafting of incident status updates to keep stakeholders informed while reducing responder overhead
• Postmortem Generation - Automated creation of incident postmortem reports using available incident data
• GenAI Assistant - A Slack-integrated chatbot providing incident-related information and support
### Early 2024 Release

• AI Automation Digest - Intelligent summarization of complex runbook job logs with actionable next steps
## Key Technical Challenges

### Technology Adoption

• Rapidly evolving LLM landscape with new models being released frequently
• Extensive learning curve for teams
• Difficulty in model selection given rapid pace of change
### Development Process

• Limited planning time due to aggressive timeline
• Multiple concurrent workstreams
• Risk of duplicate effort across teams
• Complex stakeholder management
### Technical Implementation

• Performance evaluation of LLM outputs
• Security and compliance requirements
• Monitoring and observability needs
## Solutions and Architecture

### Centralized LLM API Service

• Single point of access for all LLM functionality
• Built on Kubernetes for scalability
• Microservices architecture enabling easy provider/model switching
• Centralized security controls and monitoring
• Support for multiple LLM providers (OpenAI, AWS Bedrock)
### Key Service Components

• Authentication layer for customer verification
• LLM Manager for prompt handling and provider interaction
• Flexible endpoint system for different use cases
• Comprehensive logging and monitoring
### Security Features

• Account-level authentication
• Request throttling
• Prompt injection prevention
• Centralized security controls
• Continuous risk assessment
## Process and Organization

### Role Definition

• Applied Scientists - Feasibility evaluation and model selection
• ML Engineers - LLM API service development
• Product Managers - Use case definition
• Product Development Engineers - Feature integration
### Development Process

• Feasibility evaluation with Applied Scientists
• Security review early in process
• Design document creation
• Iterative development starting with simplest approach
• Continuous performance evaluation
## Testing and Evaluation Framework

### Manual Testing

• Internal testing using Streamlit
• "Customer Zero" program for internal feedback
• Security and compliance reviews
### Automated Testing

• Labeled datasets and benchmarks
• Implicit customer feedback monitoring
• LLM-based output comparison
• Automated metrics tracking
### Risk Management

• Threat identification per use case
• Impact assessment (reputational/financial)
• Mitigation strategy development
• Risk-effort prioritization framework
## Key Success Factors

### Organizational

• Clear role definition and responsibilities
• Strong cross-team collaboration
• Early planning despite rapid timeline
• Iterative development approach
### Technical

• Centralized LLM service architecture
• Robust security framework
• Comprehensive monitoring
• Flexible infrastructure supporting multiple providers
### Process

• Structured evaluation framework
• Clear success criteria
• Regular security reviews
• Continuous performance monitoring
## Future Considerations

• Integration of self-hosted models
• Support for fine-tuned models
• Enhanced monitoring capabilities
• Additional provider integrations
• Streaming response capabilities for specific use cases
The case study demonstrates how enterprise organizations can successfully implement LLM features in production through careful architecture decisions, clear processes, and strong organizational alignment, even under aggressive timelines.


