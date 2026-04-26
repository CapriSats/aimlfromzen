# Incident.io: Building and Deploying an AI-Powered Incident Summary Generator (2024)

https://incident.io/blog/lessons-learned-from-building-our-first-ai-product

## Short Summary

incident.io developed an AI feature to automatically generate and suggest incident summaries using OpenAI's models. The system processes incident updates, Slack conversations, and metadata to create comprehensive summaries that help newcomers get up to speed quickly. The feature achieved a 63% direct acceptance rate, with an additional 26% of suggestions being edited before use, demonstrating strong practical utility in production.

## Long Summary

# Building AI-Powered Incident Summaries at incident.io

## Overview

incident.io, an incident management platform, successfully implemented their first AI feature using OpenAI's models to automatically generate and suggest incident summaries. This case study provides valuable insights into the practical challenges and solutions in deploying LLMs in a production environment, with particular focus on prompt engineering, testing methodologies, and production deployment considerations.

## Technical Implementation Details

### System Architecture

• Built a dedicated directory structure for AI features with standardized interfaces
• Created a centralized RunPrompt entry point that handles:
### Prompt Engineering and Testing

• Developed custom tooling for prompt testing
• Utilized OpenAI's JSON mode for structured outputs
### Production Deployment Strategy

• Implemented a phased rollout approach
• Built comprehensive feedback mechanisms
### Data Processing and Integration

• Integrated with Slack API for message enrichment
• Implemented data filtering based on timestamps
• Created systems for processing incident updates and metadata
• Established zero-data retention agreement with OpenAI
## Production Considerations

### Legal and Compliance

• Implemented customer notification system for sub-processor additions
• Established data processing agreements
• Created transparent documentation addressing:
### Performance Optimization

• Optimized Slack message enrichment process
• Implemented data access patterns for efficient processing
• Created caching mechanisms where appropriate
### Monitoring and Quality Control

• Built feedback collection systems
• Implemented tracking for suggestion quality
• Created monitoring for usage patterns
• Established metrics for feature effectiveness
## Lessons Learned

### Technical Insights

• Prompt engineering requires dedicated, uninterrupted focus
• Testing infrastructure is crucial for consistent results
• Structured output formats improve reliability
• Foundation work enables faster future AI feature development
### Process Improvements

• Different project management approach needed for AI features
• Iterative development more important than in traditional software
• Importance of early legal team involvement
• Need for clear communication about timelines and expectations
### Best Practices Established

• Human oversight over automatic updates
• Comprehensive feedback mechanisms
• Structured testing approaches
• Clear documentation of data handling
• Phased rollout strategy
## Future Considerations

### Scalability

• Created reusable infrastructure for future AI features
• Established patterns for testing and deployment
• Built extensible prompt management system
### Integration Patterns

• Standardized interfaces for AI features
• Centralized prompt management
• Consistent error handling and logging
## Technical Requirements

### Infrastructure

• OpenAI API integration
• Slack API integration
• Testing frameworks
• Monitoring systems
### Data Management

• Secure storage systems
• Data enrichment pipelines
• Access control mechanisms
### Security

• Zero-data retention policies
• Encryption standards
• Access controls
• Audit logging
The case study demonstrates a successful implementation of LLMs in a production environment, with particular attention to practical considerations around testing, deployment, and monitoring. The team's approach to prompt engineering, testing infrastructure, and phased rollout provides a valuable template for other organizations looking to implement similar AI features.


