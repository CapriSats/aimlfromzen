# Thoughtworks: Building an AI Co-pilot for Product Strategy with LLM Integration Patterns (2023)

https://martinfowler.com/articles/building-boba.html

## Short Summary

Thoughtworks built Boba, an experimental AI co-pilot for product strategy and ideation, to explore effective patterns for LLM-powered applications beyond simple chat interfaces. The team developed and documented key patterns including templated prompts, structured responses, real-time progress streaming, context management, and external knowledge integration. The case study provides detailed implementation insights for building sophisticated LLM applications with better user experiences.

## Long Summary

# Building Boba: An LLM-Powered Product Strategy Co-pilot

## Project Overview

Thoughtworks developed Boba, an experimental AI co-pilot application designed to augment product strategy and creative ideation processes. The project serves as a practical exploration of building production-grade LLM applications that go beyond simple chat interfaces, incorporating sophisticated patterns for user interaction and system integration.

## Core Capabilities

• Research signals and trends analysis using web search integration
• Creative matrix generation for concept ideation
• Scenario building with different time horizons
• Strategy ideation using the Playing to Win framework
• Product concept generation
• Visual storyboarding with Stable Diffusion integration
## Key LLMOps Patterns and Implementation Details

### System Architecture and Integration

• Web application frontend with structured UI elements for task-specific interactions
• Backend integration with OpenAI's GPT-3.5/4
• Use of Langchain for prompt management and chains
• Integration with external tools including Google SERP API and vector stores
### Pattern: Templated Prompt

• Implementation using Langchain's templating system
• Focus on maintainable, single-purpose templates without complex conditionals
• Strategic use of persona adoption in prompts
• Example of practical prompt engineering workflow:
### Pattern: Structured Response

• JSON-based response formatting
• Successful implementation of complex nested schemas
• Use of pseudo-code schema descriptions in prompts
• Integration with OpenAI's Function Calling feature
• Example response structures for:
### Pattern: Real-Time Progress

• Implementation of streaming responses using OpenAI and Langchain APIs
• UI considerations for partial response display
• Progress monitoring and cancellation capabilities
• Integration with Vercel AI SDK for edge-ready streaming
• Handling of temporal state during streaming
### Pattern: Context Management

• Implementation of selection-based context carrying
• Multiple context implementation approaches:
• Integration with chat history management
### Pattern: External Knowledge Integration

• RAG (Retrieval Augmented Generation) implementation using:
• Chunking strategy for long documents:
• Integration with Langchain's VectorDBQAChain
## Technical Implementation Details

### Vector Store Integration

### Streaming Implementation

## Production Considerations

• Error handling for LLM responses
• Proper context window management
• Rate limiting and cost management
• Response validation and formatting
• Streaming state management
• UI/UX considerations for loading states
## Lessons Learned

• Importance of proper prompt engineering and testing workflow
• Value of structured responses for complex applications
• Need for robust streaming implementations
• Benefits of context management for user experience
• Significance of proper vector store integration for knowledge management
## Future Developments

• Implementation of reinforcement learning for response improvement
• Enhanced feedback mechanisms
• Improved context management systems
• Integration with additional external tools
• Enhanced visual generation capabilities
The case study demonstrates sophisticated patterns for building production-ready LLM applications, moving beyond simple chat interfaces to create powerful, context-aware tools that can effectively augment human capabilities in specific domains.


