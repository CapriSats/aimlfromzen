# Globant: LLM Production Case Studies: Consulting Database Search, Automotive Showroom Assistant, and Banking Development Tools (2023)

https://www.youtube.com/watch?v=ATYXc6mmGo0

## Short Summary

A collection of LLM implementation case studies detailing challenges and solutions in various industries. Key cases include: a consulting firm's semantic search implementation for financial data, requiring careful handling of proprietary data and similarity definitions; an automotive company's showroom chatbot facing challenges with data consistency and hallucination control; and a bank's attempt to create a custom code copilot, highlighting the importance of clear requirements and technical understanding in LLM projects.

## Long Summary

# Multiple LLM Production Case Studies: Lessons from the Field

## Overview

This case study presents multiple real-world implementations of LLM-based systems across different industries, highlighting common challenges, solutions, and key lessons learned in deploying LLMs in production environments.

## Case Study 1: Consulting Firm's Financial Database Search

### Background

• Consulting firm needed to implement semantic search functionality for a large financial database
• Database contained market caps, valuations, mergers, acquisitions, and other financial data
• Data was highly proprietary and valuable, preventing creation of supplementary databases
• Main challenge centered around text-heavy SQL database fields
### Technical Challenges

• Similarity definition problems in financial context
• Extremely low tolerance for spurious retrieval
• Requirements for quick response times
• Need for consistent results across different queries
• Unable to modify existing database structure
### Solution Implementation

• Developed text-to-SQL approach for structured data queries
• Used LLM to generate relevant keywords for search context
• Implemented post-retrieval filtering and reranking
• Lean processing to maintain performance requirements
### Key Lessons

• Most retrieval-augmented generation requires data source modification
• Business definitions of similarity differ from technical implementations
• Graph databases might be better suited than vector databases for certain use cases
• Important to establish clear validation points early in the project
## Case Study 2: Automotive Showroom Virtual Assistant

### Background

• Car manufacturer wanted to create an interactive showroom experience
• Project involved partnership with major cloud provider
• Required handling of non-canonical documentation across different countries
• Needed to maintain brand identity and handle restricted information
### Technical Challenges

• Working with legacy LLM models
• Cloud service-induced hallucinations in file search
• Restrictions on discussing certain topics (pricing, competitors)
• Complex comparison requirements against unrestricted chatbots
### Solution Implementation

• Implemented multi-layer LLM processing
• Created custom document summarization pipeline
• Developed strict hallucination prevention mechanisms
• Built custom metadata generation system
### Key Lessons

• Critical importance of measuring at every processing stage
• Need to break down RAG systems into measurable components
• Importance of canonical data sources
• Value of clear documentation and source truth
## Case Study 3: Information and Sales Assistant

### Background

• Project aimed to leverage success cases and industry reports
• Built in early 2023 with less mature frameworks
• Needed to handle both technical reports and success cases
• Required measurable effectiveness metrics
### Technical Challenges

• Different document formats requiring different processing approaches
• Complex source selection logic
• Difficulty in measuring effectiveness
• Limited access to source format information
### Solution Implementation

• Combined vector search with structured SQL database approach
• Implemented agentic workflows for quality improvement
• Created custom pre-structuring for document processing
### Key Lessons

• Not all solutions require vector databases
• Engineering work often more challenging than LLM integration
• Importance of proper data access and processing pipelines
## Case Study 4: Banking Code Copilot

### Background

• International bank wanted custom GitHub Copilot alternative
• Initially restricted to GPT-3.5 due to budget constraints
• Lack of clear success metrics
• Limited understanding of fine-tuning requirements
### Key Lessons

• Importance of clear requirements and success metrics
• Need for technical expertise in project planning
• Value of setting realistic expectations
• Risk management in client relationships
## Overall LLMOps Lessons

### Technical Considerations

• Importance of proper evaluation frameworks
• Need for robust testing and validation
• Value of systematic measurement and monitoring
• Consideration of multiple architectural approaches
### Organizational Considerations

• Clear communication of technical limitations
• Importance of setting realistic expectations
• Need for proper expertise in project planning
• Value of challenging unrealistic requirements
### Implementation Best Practices

• Systematic measurement at every stage
• Clear documentation and source truth
• Proper handling of proprietary data
• Robust testing and validation frameworks

