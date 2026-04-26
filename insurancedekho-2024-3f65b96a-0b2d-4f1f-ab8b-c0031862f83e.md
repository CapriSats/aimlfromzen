# InsuranceDekho: Transforming Insurance Agent Support with RAG-Powered Chat Assistant (2024)

https://aws.amazon.com/blogs/machine-learning/how-insurancedekho-transformed-insurance-agent-interactions-using-amazon-bedrock-and-generative-ai?tag=soumet-20

## Short Summary

InsuranceDekho addressed the challenge of slow response times in insurance agent queries by implementing a RAG-based chat assistant using Amazon Bedrock and Anthropic's Claude Haiku. The solution eliminated the need for constant SME consultation, cached frequent responses using Redis, and leveraged OpenSearch for vector storage, resulting in an 80% reduction in response times for customer queries about insurance plans.

## Long Summary

# Transforming Insurance Agent Support with RAG and Generative AI at InsuranceDekho

## Company Background and Challenge

InsuranceDekho is a leading InsurTech service in India that works with over 49 insurance companies through a network of 150,000 point of sale person (POSP) agents. The company faced a significant operational challenge where insurance advisors, especially newcomers, frequently needed to consult subject matter experts (SMEs) for policy-specific queries. This dependency created delays in customer response times and increased operational costs.

## Technical Solution Architecture

### Core Technology Stack

• Foundation Model Platform: Amazon Bedrock
• Large Language Model: Anthropic's Claude Haiku
• Vector Database: Amazon OpenSearch Service
• Caching Layer: Redis on Amazon ElastiCache
• Third-party embedding model for vector transformations
### Implementation Workflows

The solution comprises two main workflows:

### Data Ingestion Workflow

• Policy documents are processed through embedding models
• Vector representations are stored in OpenSearch Service
• Continuous updates maintain knowledge base currency
### Query Response Workflow

• Chatbot interface for insurance advisor interactions
• Redis-based caching system for frequent queries
• Intent classification using Claude Haiku
• RAG-based context retrieval and response generation
• Dynamic prompting based on query type
## Key Technical Decisions and Rationale

### Amazon Bedrock Selection

• Serverless Architecture: Eliminated need for infrastructure management
• Model Flexibility: Single API access to multiple foundation models
• Easy Model Switching: Demonstrated by smooth transition from Claude Instant to Claude Haiku
• Security: AWS PrivateLink integration for private model access
• Performance Options: Both on-demand and provisioned throughput available
### Performance Optimization Strategies

• Caching Layer Implementation
• Intent Classification
### Vector Database Implementation

• OpenSearch Service chosen for:
## Production Deployment Considerations

### Security and Compliance

• Private model access through AWS PrivateLink
• Secure data transfer for inference
• Compliance adherence in data handling
### Performance Monitoring

• Response time tracking
• Cache hit rates
• Query classification accuracy
• Vector search performance
### Scalability Design

• Serverless architecture for variable load handling
• Elastic cache scaling
• Vector database performance optimization
## Results and Impact

### Performance Improvements

• 80% reduction in query response times
• Significant decrease in SME dependencies
• Enhanced agent confidence and autonomy
### Business Benefits

• Improved customer service efficiency
• Reduced operational costs
• Better scalability of support operations
• Enhanced accuracy in policy information delivery
## Technical Learnings and Best Practices

### RAG Implementation

• Importance of quality embeddings
• Context window optimization
• Prompt engineering for accurate responses
### System Integration

• Seamless integration between multiple AWS services
• Effective caching strategies
• Query optimization techniques
### Model Selection and Evaluation

• Benchmarking process for LLM selection
• Performance metrics consideration
• Cost-effectiveness analysis
## Future Considerations

### Potential Enhancements

• Continuous model updates and evaluations
• Enhanced caching strategies
• Advanced intent classification
• Expanded knowledge base coverage
### Scalability Planning

• Load balancing improvements
• Cache optimization
• Vector database performance tuning
## Technical Architecture Details

### Data Flow

• Query input through chatbot interface
• Cache check with semantic search
• Intent classification processing
• Context retrieval from vector database
• Response generation and delivery
### System Components

• Frontend chatbot interface
• Caching layer with Redis
• Vector database with OpenSearch
• LLM integration through Amazon Bedrock
• Intent classification system
### Monitoring and Maintenance

• Performance metrics tracking
• Cache hit rate monitoring
• Response accuracy evaluation
• System health checks
• Knowledge base updates

