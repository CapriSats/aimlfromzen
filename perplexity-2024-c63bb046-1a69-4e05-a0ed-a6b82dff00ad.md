# Perplexity: Building a Complex AI Answer Engine with Multi-Step Reasoning (2024)

https://www.langchain.com/breakoutagents/perplexity

## Short Summary

Perplexity developed Pro Search, an advanced AI answer engine that handles complex, multi-step queries by breaking them down into manageable steps. The system combines careful prompt engineering, step-by-step planning and execution, and an interactive UI to deliver precise answers. The solution resulted in a 50% increase in query search volume, demonstrating its effectiveness in handling complex research questions efficiently.

## Long Summary

# Perplexity Pro Search: Advanced AI Answer Engine Implementation

## System Overview

Perplexity has developed Pro Search, an advanced AI answer engine designed to handle complex queries requiring multi-step reasoning. Unlike traditional search engines or basic AI search tools, Pro Search specializes in breaking down and answering nuanced questions that require connecting multiple pieces of information.

## Technical Architecture

### Cognitive System Design

• Implements a distinct separation between planning and execution phases
• Planning phase:
• Execution phase:
### Specialized Tool Integration

• Incorporates code interpreters for real-time calculations
• Integration with Wolfram Alpha for mathematical evaluations
• Support for various specialized tools based on query requirements
## LLM Implementation

### Model Selection and Management

• Utilizes multiple language models for different search tasks
• Users can select models based on specific problem requirements
• Backend customization of prompts for each individual model
### Prompt Engineering Strategies

• Implementation of few-shot prompt examples
• Utilization of chain-of-thought prompting
• Key considerations in prompt design:
## Quality Assurance and Evaluation

### Testing Methodology

• Comprehensive manual evaluations
### Automated Evaluation

• Large-scale question batch testing
• Implementation of LLM-as-a-Judge for answer ranking
• Extensive A/B testing focusing on:
## User Experience Design

### Interactive Interface

• Development of dynamic progress display
• Implementation of expandable sections for detailed step viewing
• Citation system with hover functionality
• Source snippet preview capability
### UX Optimization

• Progressive information disclosure
• Balance between simplicity and functionality
• Multiple iteration cycles for interface refinement
• Focus on accommodating users with varying AI expertise levels
## Production Implementation

### Performance Metrics

• Achieved 50% increase in query search volume
• Continuous monitoring of:
### System Architecture Considerations

• Balance between speed and accuracy
• Optimization of intermediate step processing
• Integration of multiple specialized tools
• Efficient document retrieval and ranking system
## DevOps and Deployment

### Development Process

• Iterative development approach
• Continuous testing and refinement
• Internal dogfooding before feature release
• Regular evaluation of system components
### Production Monitoring

• Answer quality tracking
• User interaction analysis
• Performance metrics monitoring
• System reliability assessment
## Best Practices and Lessons Learned

### Key Insights

• Importance of explicit planning steps for complex queries
• Critical balance between speed and answer quality
• Value of transparent intermediate steps
• Necessity of user-centric design
### Implementation Guidelines

• Keep prompt instructions simple and precise
• Maintain clear separation between planning and execution
• Provide progressive feedback to users
• Design for users with varying technical expertise
## Future Considerations

### Scaling Strategies

• Continuous refinement of evaluation methods
• Expansion of specialized tool integration
• Enhancement of user interface capabilities
• Optimization of processing efficiency
### Product Evolution

• Regular updates based on user feedback
• Continuous improvement of answer quality
• Enhancement of interactive features
• Expansion of supported query types

