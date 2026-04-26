# Various: Production LLM Systems: Document Processing and Real Estate Agent Co-pilot Case Studies (2023)

https://www.youtube.com/watch?v=ll-Xit_Khq0

## Short Summary

A comprehensive webinar featuring two case studies of LLM systems in production. First, Docugami shared their experience building a document processing pipeline that leverages hierarchical chunking and semantic understanding, using custom LLMs and extensive testing infrastructure. Second, Reet presented their development of Lucy, a real estate agent co-pilot, highlighting their journey with OpenAI function calling, testing frameworks, and preparing for fine-tuning while maintaining production quality.

## Long Summary

# Production LLM Systems Case Studies

## Overview

This case study presents insights from two companies implementing LLMs in production: Docugami and Reet. Both companies shared their experiences during a webinar, focusing on different aspects of LLMOps and production challenges.

## Docugami's Document Processing System

### Document Processing Challenges

• Complex document structures requiring both structural and semantic understanding
• Need for hierarchical chunking and knowledge representation
• Handling non-linear layouts, tables, and multi-column documents
• Managing complex chains and parallel processing
### Technical Implementation

• Built custom XML-based knowledge graph for document representation
• Implemented structural chunking based on document layout
• Used Apache Spark as execution engine
• Deployed models in Kubernetes cluster
• Leveraged Nvidia Triton for model hosting
• Utilized Redis for vector database and caching
### LLMOps Infrastructure

• Developed custom LLM deployment for efficiency
• Used smaller fine-tuned models for specific tasks
• Implemented larger models for more complex interactions
• Regular monitoring of failed runs and user feedback
• Created datasets in LangSmith for continuous improvement
• Used larger LLMs offline to propose fixes for smaller model mistakes
### Testing and Quality Assurance

• Implemented comprehensive testing infrastructure
• Used LangSmith for debugging and tracing
• Added user feedback mechanisms (thumbs up/down)
• Created data sets from problematic runs
• Performed post-processing validation for syntactic correctness
### Continuous Improvement Process

• Regular review of failed runs
• Collection of user feedback
• Dataset creation and maintenance
• Model fine-tuning based on collected data
• Deployment of improved models
## Reet's Real Estate Agent Co-pilot (Lucy)

### System Overview

• Built Lucy as a comprehensive co-pilot for real estate agents
• Initially used LangChain's structured chat agent
• Transitioned to OpenAI function calling for improved performance
• Focused on developer experience and testing infrastructure
### Technical Challenges

• Initial implementation was too slow with structured chat agent
• Function calling improved latency 3-4x but still had reliability issues
• Needed robust testing framework for non-deterministic outputs
• Required extensive prompt engineering and fine-tuning preparation
### Testing Infrastructure

• Created custom test runner for concurrent testing
• Generated synthetic test cases
• Implemented CI/CD pipeline with detailed logging
• Integrated with LangSmith for debugging and reproduction
### Development Process

• Quick integration with LangSmith (under 5 minutes)
• Added detailed tags and metadata for tracking
• Created playground environment for quick iteration
• Implemented comprehensive logging and debugging capabilities
### Data Collection and Fine-tuning Strategy

• Created separate databases for good and bad samples
• Implemented manual curation process
• Planning for GPT-3.5 fine-tuning with function calling
• Built pipeline for data preparation and processing
### Key Learnings

• Best practices are still evolving
• Tooling landscape is rapidly changing
• Not everything needs to be fully automated
• Importance of staying open to change and new solutions
• Critical role of human oversight in quality assurance
## Shared Challenges and Solutions

### Performance and Reliability

• Both companies focused on achieving production-grade reliability
• Implemented extensive testing and monitoring
• Used custom models and infrastructure where needed
• Balanced automation with human oversight
### Data Management

• Importance of versioning datasets
• Need for robust data collection pipelines
• Value of human review in data curation
• Integration with existing tools and frameworks
### Infrastructure Decisions

• Careful consideration of hosting vs. API usage
• Focus on cost management and scaling
• Implementation of comprehensive monitoring
• Integration with existing development workflows
### Future Considerations

• Preparing for rapid tooling evolution
• Planning for improved fine-tuning capabilities
• Building flexible and adaptable systems
• Maintaining focus on end-user experience
The case studies demonstrate the complexity of deploying LLMs in production and the importance of building robust infrastructure for testing, monitoring, and continuous improvement. Both companies emphasized the need for flexible systems that can adapt to rapidly evolving best practices and tooling in the LLMOps space.


