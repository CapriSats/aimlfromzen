# Schneider Electric: Retrieval Augmented LLMs for Real-time CRM Account Linking (2023)

https://aws.amazon.com/blogs/machine-learning/schneider-electric-leverages-retrieval-augmented-llms-on-sagemaker-to-ensure-real-time-updates-in-their-crm-systems?tag=soumet-20

## Short Summary

Schneider Electric partnered with AWS Machine Learning Solutions Lab to automate their CRM account linking process using Retrieval Augmented Generation (RAG) with Flan-T5-XXL model. The solution combines LangChain, Google Search API, and SEC-10K data to identify and maintain up-to-date parent-subsidiary relationships between customer accounts, improving accuracy from 55% to 71% through domain-specific prompt engineering.

## Long Summary

# Schneider Electric's RAG Implementation for CRM Account Linking

## Overview and Business Challenge

Schneider Electric, a leader in energy management and industrial automation, faced a significant challenge in maintaining accurate relationships between customer accounts across their CRM systems. As their customer base grew, account teams had to manually process new customers and link them to appropriate parent entities. This process required constant attention to the latest information from various sources, including acquisitions, market news, and organizational restructuring.

## Technical Solution Architecture

### LLM Selection and Deployment

• Utilized Flan-T5-XXL model from the Flan-T5 family
• Model deployed through Amazon SageMaker JumpStart
• Selected for its strong performance in question-answering tasks with provided context
• 11B parameter model proved sufficient for the specific use case
• Deployed as a SageMaker endpoint for inference
### RAG Implementation with LangChain

• Leveraged LangChain framework for orchestrating the RAG pipeline
• Implemented two main components:
• Integration with multiple data sources:
### Pipeline Architecture

• Two-step process implementation:
• Used LangChain chains to combine different components:
• Incorporated pandas dataframe agent for structured data processing
## Prompt Engineering Innovations

### Domain-Specific Prompts

• Initial generic prompts showed limited effectiveness
• Developed sector-specific prompts for different industries:
• Implementation of domain classification step:
• Achieved significant improvement in accuracy:
### Data Integration Techniques

### Google Search Integration

• Real-time information retrieval through Google Serper API
• Custom prompt templates for search result processing
• Dynamic query construction based on company names
### SEC-10K Data Processing

• Tabular data integration through LangChain's pandas dataframe agent
• Natural language interface for data querying
• Robust handling of variations in company names and misspellings
• Combination of structured and unstructured data sources
## Technical Implementation Details

### Code Architecture

• Modular design with separate components for:
• Flexible configuration for different data sources
• Error handling and fallback mechanisms
### Performance Optimization

• Efficient prompt template design
• Structured response formatting
• Caching mechanisms for frequently accessed data
• Parallel processing where applicable
### Deployment and Monitoring

• SageMaker endpoint deployment
• Integration with existing CRM systems
• Performance tracking and accuracy measurements
• Regular model and prompt updates
## Results and Impact

### Performance Metrics

• Accuracy improvement from 55% to 71%
• Significant reduction in manual processing time
• Improved data consistency across CRM systems
### Business Benefits

• Real-time account relationship updates
• Reduced manual effort for account teams
• More accurate downstream analytics
• Improved customer data management
## Technical Challenges and Solutions

### Data Quality and Integration

• Handling inconsistent company names
• Managing multiple data sources
• Resolving conflicting information
• Implementing verification mechanisms
### System Architecture

• Scalable design for growing customer base
• Integration with existing systems
• Managing API rate limits
• Ensuring system reliability
## Future Enhancements

### Planned Improvements

• Enhanced prompt customization capabilities
• Additional data source integration
• Improved accuracy metrics
• Expanded domain coverage
### Scalability Considerations

• System architecture optimization
• Performance monitoring
• Resource utilization management
• Cost optimization strategies

