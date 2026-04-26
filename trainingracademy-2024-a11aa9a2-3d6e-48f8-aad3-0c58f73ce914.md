# Trainingracademy: Building a RAG System for Cybersecurity Research and Reporting (2024)

https://www.youtube.com/watch?v=_uPWW0ExiPw

## Short Summary

TrainGRC developed a Retrieval Augmented Generation (RAG) system for cybersecurity research and reporting to address the challenge of fragmented knowledge in the cybersecurity domain. The system tackles issues with LLM censorship of security topics while dealing with complex data processing challenges including PDF extraction, web scraping, and vector search optimization. The implementation focused on solving data quality issues, optimizing search quality through various embedding algorithms, and establishing effective context chunking strategies.

## Long Summary

# RAG Implementation for Cybersecurity Knowledge Base at TrainGRC

## Company Overview and Problem Statement

TrainGRC, a startup focused on cloud security training, developed a platform called stinkbait.io for cybersecurity research and reporting. The company faced several unique challenges in the cybersecurity domain:

• Knowledge fragmentation across different subcommunities
• LLM censorship of security-related topics
• Need for accurate and comprehensive information sharing
## Technical Implementation Challenges

### Data Quality Management

### PDF Processing Challenges

• Historical context: PDFs have existed since 1993 with numerous extensions
• Common issues:
### PDF Processing Solution

• Primary tool: Amazon Textract for OCR
• Fallback strategy:
### Web Scraping Challenges

• Inconsistent HTML structure across sources
• Various web frameworks and WYSIWYG editors
• Poor data structure standardization
### Web Scraping Solution

• Manual inspection of websites required
• Custom parsing based on specific HTML elements
• Careful validation of extracted data quality
• Avoiding reliance on generic third-party tools
### Search Quality Optimization

### Vector Search Algorithm Considerations

• Trade-offs between exact KNN and approximate nearest neighbor searches
• Implementation options:
### Database Technology Selection

• Initial approach:
• Challenges encountered:
### Vector Database Considerations

• Evaluation criteria:
• Decision factors:
### Embedding Model Selection

### Model Options Analysis

• Default choice: Ada embeddings
### Specialized Models Consideration

• Types of embedding models:
### Context Management

### Context Chunking Strategies

• Ideal approach:
• Practical implementation:
### Long-term Storage Considerations

• Vector storage strategy:
### Model Migration Planning

• Key considerations:
## Implementation Lessons

### Best Practices

• Importance of upfront data quality
• "Garbage in, garbage out" principle
• Need for manual inspection and validation
• Balance between automation and quality control
### Future Considerations

• Active research in context boundary detection
• Evolution of embedding models
• Continuous evaluation of vector database solutions
• Adaptation to changing security landscape
## Technical Infrastructure

### Tools and Technologies

• Amazon Textract for OCR
• Vector databases
• Embedding models (Ada and alternatives)
• Custom data processing pipelines
• Storage solutions for vectors and raw data
### Architecture Decisions

• Modular approach to data processing
• Flexible storage solutions
• Scalable vector search implementation
• Backup strategies for data extraction

