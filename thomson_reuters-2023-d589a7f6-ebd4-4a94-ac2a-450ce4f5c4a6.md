# Thomson Reuters: Enterprise LLM Playground Development for Internal AI Experimentation (2023)

https://aws.amazon.com/blogs/machine-learning/how-thomson-reuters-developed-open-arena-an-enterprise-grade-large-language-model-playground-in-under-6-weeks?tag=soumet-20

## Short Summary

Thomson Reuters developed Open Arena, an enterprise-wide LLM playground, in under 6 weeks using AWS services. The platform enables non-technical employees to experiment with various LLMs in a secure environment, combining open-source and in-house models with company data. The solution saw rapid adoption with over 1,000 monthly users and helped drive innovation across the organization by allowing safe experimentation with generative AI capabilities.

## Long Summary

# Thomson Reuters Open Arena: Enterprise LLM Platform Case Study

## Company Background and Context

Thomson Reuters has a long history of integrating AI into their professional information products, dating back to 1992 with their Westlaw Is Natural (WIN) system. In 2023, they sought to democratize access to LLM experimentation across their organization while maintaining enterprise-grade security and control.

## The Challenge

The company needed to:

• Enable non-technical employees to experiment with LLMs
• Provide a secure environment for testing both open-source and in-house models
• Allow exploration of use cases combining LLMs with company data
• Maintain security and compliance requirements
• Deploy rapidly to keep pace with fast-moving LLM developments
## Technical Architecture and Implementation

### Core Infrastructure

• Built on AWS serverless architecture for scalability and cost-effectiveness
• Used Amazon SageMaker as the primary model deployment platform
• Leveraged Hugging Face Deep Learning Containers for simplified deployment
• Implemented API Gateway and Lambda functions for request handling
• Utilized DynamoDB for storing user interactions and metadata
• Deployed frontend as static site on S3 with CloudFront distribution
### Model Development and Deployment

• Integrated multiple LLM types:
• Implemented quantization using bitsandbytes for performance optimization
• Used Hugging Face Inference Toolkit and Accelerate library for efficient inference
### Security and Compliance

• All data encrypted and contained within VPC
• Company SSO integration for access control
• Secure API endpoints
• Monitored usage through CloudWatch
• Controlled data access and model permissions
### RAG Implementation

• Document processing pipeline for content integration
• Chunk-based document splitting
• Embedding generation and storage in OpenSearch
• Bi-encoder and cross-encoder based retrieval/re-ranking
• Context-aware response generation
## DevOps and MLOps Practices

• CI/CD pipeline using AWS CodeBuild and CodePipeline
• Comprehensive monitoring with CloudWatch dashboards
• Automated deployment processes
• Usage tracking and analytics
• Performance monitoring and optimization
## User Interface and Experience

### Tile-Based Interface

• Pre-configured experiences for different use cases
• Chat-like interaction channels
• Document upload and query capabilities
• Summarization tools
• Simple, intuitive design for non-technical users
## Results and Impact

### Quantitative Metrics

• Developed in under 6 weeks
• Over 1,000 monthly active users
• Average 5-minute interaction time per user
• Global adoption across company divisions
### Qualitative Outcomes

• Increased AI awareness and literacy across organization
• Generated numerous new use cases for LLM application
• Improved cross-team collaboration
• Accelerated AI innovation cycle
• Positive user feedback from diverse departments
## Technical Lessons and Best Practices

### Architecture Decisions

• Serverless architecture proved effective for rapid scaling
• Modular design allowed quick integration of new models
• API-first approach enabled flexible frontend development
• Emphasis on security from initial design
### Implementation Insights

• Importance of model evaluation for specific use cases
• Balance between model size and performance requirements
• Need for robust monitoring and usage tracking
• Value of user feedback in feature development
## Ongoing Development

### Current Focus Areas

• Integration with newer AWS services (Amazon Bedrock, SageMaker JumpStart)
• Expanding model offerings
• Enhancing RAG capabilities
• Performance optimization
• User experience improvements
### Future Roadmap

• Productionization of successful use cases
• Enhanced monitoring and analytics
• Additional security features
• Expanded integration capabilities
## Critical Success Factors

• Strong AWS service integration
• Focus on security and compliance
• User-centric design approach
• Rapid development and deployment
• Effective change management and training
• Support from leadership
• Clear communication and documentation
## Challenges and Solutions

### Technical Challenges

• Model performance optimization
• Secure data handling
• Scalability requirements
• Integration complexity
### Solutions Implemented

• Quantization techniques for model optimization
• VPC-based security architecture
• Serverless scaling approach

