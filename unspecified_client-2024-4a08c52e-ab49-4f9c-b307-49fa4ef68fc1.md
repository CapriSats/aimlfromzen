# Unspecified client: Building a Financial Data RAG System: Lessons from Search-First Architecture (2024)

https://www.linkedin.com/pulse/my-first-rag-use-case-key-insights-lessons-learned-dan-giannone-sa7ne/

## Short Summary

A case study of implementing a RAG-based chatbot for financial executives and analysts to access company data across SEC filings, earnings calls, and analyst reports. The team initially faced challenges with context preservation, search accuracy, and response quality using standard RAG approaches. They ultimately succeeded by reimagining the search architecture to focus on GPT-4 generated summaries as the primary search target, along with custom scoring profiles and sophisticated prompt engineering techniques.

## Long Summary

# Building a Financial RAG System with Search-First Architecture

## Project Overview

This case study details the implementation of a RAG-based chatbot system for financial executives, finance teams, and investor relations departments at a major client. The system was designed to help users quickly access and analyze information across SEC filings, earnings calls, analyst reports, and internal financial documents.

## Technical Architecture

• Azure OpenAI Service with GPT-4-32k and GPT-4-Turbo models
• Azure AI Search for document indexing and retrieval
• Azure App Service for the web application backend
• Python-based implementation using Microsoft's accelerator template
## Key Challenges and Solutions

### Initial Implementation Challenges

• Context preservation issues when chunking documents
• Incorrect attribution of quotes and financial data
• Poor search result quality mixing disclaimers with actual content
• Inability to handle multi-entity queries effectively
• Lack of temporal understanding in search results
### Search Architecture Innovation

The team developed a novel search-first approach:

• Using GPT-4 to generate concise summaries of each document page
• Adding summaries as searchable fields in Azure AI Search index
• Vectorizing summaries instead of raw content
• Matching user queries against summary vectors for improved relevance
• Implementing custom scoring profiles based on document recency
### Content Processing Pipeline

• Page-level chunking to preserve context instead of token-based chunking
• Pre-processing step to remove problematic footers and headers
• Summary generation with specialized prompts
• Hybrid search combining vector and keyword approaches
• Custom filters to remove disclaimer/certification pages
### Query Processing Improvements

• Decision agent to determine optimal search strategy
• Breaking complex multi-entity queries into sub-queries
• Category-based filtering system
• Implementation of recency boosts in search scoring
## Technical Implementation Details

### Document Processing

• Modified chunking strategy to preserve page-level context
• Added metadata extraction including creation dates and document categories
• Implemented custom scoring profiles in Azure AI Search
• Built specialized prompting system for page summarization
### Search Optimization

• Hybrid search combining vector and keyword approaches
• Custom boosting based on document recency
• Category-based filtering system
• Context-aware search routing based on query type
### LLM Integration

• Multiple GPT-4 specialized agents:
• Prompt engineering for detailed responses
• Streaming response implementation
### System Architecture Improvements

• Implementation of caching strategies
• Addition of custom scoring profiles
• Category-based document filtering
• Temporal awareness through custom boost functions
## Project Outcomes

### Key Achievements

• Successful deployment of production RAG system
• Significant improvement in response accuracy and relevance
• Reduction in manual research time for financial analysts
• Positive user feedback on system performance
### Technical Learnings

• Importance of search quality over LLM capabilities
• Value of context preservation in document processing
• Need for specialized handling of financial data
• Benefits of hybrid search approaches
## Operational Considerations

### Production Readiness

• Need for comprehensive testing framework
• Importance of LLMOps practices
• Requirements for automated data ingestion
• Security model considerations
### Performance Optimization

• Response latency improvements
• Streaming implementation
• Caching strategies
• PTU considerations for Azure OpenAI
## Best Practices and Recommendations

### RAG Implementation

• Focus on search quality first
• Preserve document context
• Implement hybrid search approaches
• Use specialized agents for different tasks
### System Design

• Plan for scalability
• Consider security requirements early
• Implement comprehensive testing
• Build in monitoring and evaluation
### Data Processing

• Carefully consider chunking strategies
• Preserve metadata and context
• Implement proper preprocessing
• Consider domain-specific requirements
## Future Improvements

### Planned Enhancements

• Implementation of vision capabilities
• Database connectivity
• Autonomous agents
• Whole document summarization
• User document upload capability
### Technical Debt

• Testing framework implementation

