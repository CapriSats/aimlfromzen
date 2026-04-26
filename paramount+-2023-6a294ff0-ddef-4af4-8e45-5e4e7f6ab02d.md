# Paramount+: Video Content Summarization and Metadata Enrichment for Streaming Platform (2023)

https://www.youtube.com/watch?v=lGxwqCBBXwY

## Short Summary

Paramount+ partnered with Google Cloud Consulting to develop two key AI use cases: video summarization and metadata extraction for their streaming platform containing over 50,000 videos. The project used Gen AI jumpstarts to prototype solutions, implementing prompt chaining, embedding generation, and fine-tuning approaches. The system was designed to enhance content discoverability and personalization while reducing manual labor and third-party costs. The implementation included a three-component architecture handling transcription creation, content generation, and personalization integration.

## Long Summary

# Building AI-Powered Content Understanding at Paramount+

## Project Overview

Paramount+ partnered with Google Cloud Consulting to enhance their streaming platform's user experience through two primary AI use cases:

• Video summarization
• Metadata extraction and enrichment
The project aimed to process over 50,000 videos, replacing expensive and time-consuming manual processes while improving content discoverability and personalization capabilities.

## Business Context and Objectives

### Strategic Goals

• Expand subscriber base
• Improve viewer retention
• Boost engagement
• Drive profitability
### Technical Challenges

• Processing large volume of content (50,000+ videos)
• Reducing dependency on costly third-party metadata services
• Handling various content types and genres
• Managing mature content appropriately
• Dealing with long transcripts within token limits
## Implementation Approach

### Development Process

• Used Google Cloud's Gen AI jumpstart program for rapid prototyping
• Iterative development with multiple feedback cycles
• Four iterations to refine MVP prompts
• Close collaboration between Paramount+ and Google Cloud teams
### Architecture Components

The system consists of three main components:

• Transcription Creation
• Generation Phase
• Personalization Component
### Technical Implementation Details

### LLM Usage and Optimization

• Implemented prompt chaining for better control and debugging
• Careful management of token limits and context windows
• Used temperature and sampling parameters (top_p, top_k) optimization
• Generated embeddings from transcripts with dimension optimization
• Utilized smaller models (e.g., Gemma 2B) for specific tasks
### Fine-tuning Process

• Created human preference datasets
• Implemented reward model training
• Continuous model weight updates
• Evaluation dataset for performance monitoring
• Support for T5 and Gemma model types
## Best Practices and Lessons Learned

### Data Preparation

• Early access to representative video content
• Diverse content selection for testing
• Clear definition of expected metadata outputs
• Structured feedback collection process
### Prompt Engineering

• Template-based prompt management
• Genre-specific prompt classification
• Audience affinity consideration
• Clear context and specific examples inclusion
### Production Considerations

• Dynamic metadata key-value pairs for personalization
• Accessibility-focused metadata generation
• Integration with existing personalization systems
• Automated quality checks and validation
## Technical Innovations

### Model Selection and Optimization

• Used multiple model types for different tasks
• Implemented embedding space optimization
• Developed agent-like system architecture
• Integrated function calling for external data sources
### Quality Control

• Established gold standards for generated output
• Implemented evaluation datasets
• Created feedback loops for continuous improvement
• Built automated validation systems
## Results and Impact

### Technical Achievements

• Successfully automated video summarization
• Reduced dependency on manual processing
• Improved metadata quality and granularity
• Enhanced personalization capabilities
### System Improvements

• Better content discoverability
• More nuanced content understanding
• Improved user experience
• Cost reduction in metadata procurement
## Future Developments

### Planned Enhancements

• Implementation of chain prompt templates
• Development of candidate selection strategies
• Further fine-tuning of models
• Enhanced personalization features
### Architectural Evolution

• Move towards agent-based architecture
• Improved embedding space optimization
• Enhanced integration with personalization systems
• Expanded metadata generation capabilities
## Key Takeaways

### Technical Insights

• Importance of prompt engineering and iteration
• Value of structured architecture
• Need for robust evaluation systems
• Benefits of modular design
### Operational Learnings

• Early feedback collection is crucial
• Diverse content testing is essential

