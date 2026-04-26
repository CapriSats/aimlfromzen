# New Computer: Enhancing Memory Retrieval Systems Using LangSmith Testing and Evaluation (2024)

https://blog.langchain.dev/customers-new-computer/

## Short Summary

New Computer improved their AI assistant Dot's memory retrieval system using LangSmith for testing and evaluation. By implementing synthetic data testing, comparison views, and prompt optimization, they achieved 50% higher recall and 40% higher precision in their dynamic memory retrieval system compared to their baseline implementation.

## Long Summary

# Improving Memory Retrieval Systems with LangSmith: New Computer Case Study

## Company Overview and Challenge

New Computer is the developer of Dot, an advanced personal AI assistant designed to understand users deeply through a sophisticated memory system. The company faced the challenge of improving their dynamic memory retrieval system while maintaining user privacy and ensuring accurate, personalized responses.

## Technical Architecture and Implementation

### Agentic Memory System

• Implemented a novel agentic memory system that goes beyond traditional RAG
• System dynamically creates and pre-calculates documents for future retrieval
• Includes meta-fields for enhanced retrieval capabilities:
### Memory Retrieval Methods

• Implemented multiple retrieval techniques:
• Combined approaches for different query types
• Used performance metrics:
## LLMOps Implementation Details

### Testing Infrastructure

• Created synthetic test data to preserve user privacy
• Developed in-house tool connected to LangSmith for:
### Experimentation Process

• Established baseline using simple semantic search
• Conducted parallel testing of different retrieval methods
• Used LangSmith's SDK and Experiments UI for:
• Implemented combination of methods based on query types:
### Prompt Engineering and Optimization

• Developed dynamic conversational prompt system
• Integrated multiple components:
• Used LangSmith's comparison view to:
• Utilized built-in prompt playground for:
## Results and Metrics

### Performance Improvements

• Achieved 50% higher recall compared to baseline
• Obtained 40% higher precision in dynamic memory retrieval
• Demonstrated successful handling of diverse query types
• Maintained system performance across prompt variations
### Business Impact

• Successfully launched to new users
• Achieved 45% conversion rate to paid tier
• Established foundation for scalable personalization
## Production Monitoring and Maintenance

### Quality Assurance

• Continuous monitoring of retrieval performance
• Regular evaluation of prompt effectiveness
• Systematic regression testing through LangSmith
### System Scalability

• Designed for growing user base
• Implemented efficient memory management
• Maintained performance with increasing memory accumulation
## Future Developments

### Planned Enhancements

• User preference adaptation
• Proactive user engagement
• Deeper relationship simulation
### Technical Roadmap

• Continued integration with LangChain ecosystem
• Enhanced use of LangSmith for system optimization
• Development of more sophisticated retrieval methods
• Expansion of synthetic testing capabilities
## Technical Infrastructure

### Tools and Technologies

• LangSmith for testing and evaluation
• Custom-built memory management system
• Integration with LangChain framework
• Synthetic data generation pipeline
• Performance monitoring dashboard
### Best Practices Implementation

• Comprehensive testing methodology
• Privacy-preserving development approach
• Systematic experimentation process
• Data-driven optimization strategy
• Continuous performance monitoring

