# IncludedHealth: Building a Comprehensive LLM Platform for Healthcare Applications (2024)

https://includedhealth.com/blog/tech/building-a-platform-for-genai-at-included-health/

## Short Summary

IncludedHealth built Wordsmith, a comprehensive platform for GenAI applications in healthcare, starting in early 2023. The platform includes a proxy service for multi-provider LLM access, model serving capabilities, training and evaluation libraries, and prompt engineering tools. This enabled multiple production applications including automated documentation, coverage checking, and clinical documentation, while maintaining security and compliance in a regulated healthcare environment.

## Long Summary

IncludedHealth, a healthcare technology company, embarked on a significant initiative to build a comprehensive LLM platform called Wordsmith to support various AI applications across their organization. This case study provides valuable insights into building and scaling LLM operations in a regulated healthcare environment, with particular attention to security, compliance, and practical implementation challenges.

The journey began in early 2023 when the Data Science Platform team started exploring recent developments in NLP, coinciding with the release of GPT-4. The team identified several promising use cases, including knowledge base integration, intent classification, and automated documentation for healthcare providers. This exploration led to the development of Wordsmith, a platform designed to handle any text-based AI tasks while maintaining ease of use for other teams.

## Platform Architecture and Components

The platform consists of five main components, each addressing specific needs in the LLM pipeline:

### Proxy Service and Client Library

A central architectural decision was implementing a server-side proxy service that routes all LLM requests through a single internal service. This approach offers several advantages:

• Centralized credential management for different providers (OpenAI, Google, AWS)
• Consistent interface using the OpenAI API specification
• Easy provider switching without client code changes
• Cross-language support through standard OpenAI client libraries
The proxy service supports multiple providers including OpenAI, Google VertexAI, AWS Bedrock, and internal model serving, demonstrating a robust multi-vendor strategy that prevents vendor lock-in.

### Model Serving Infrastructure

The team deployed MLServer internally using HuggingFace runtime for model serving, integrated with MLFlow for model artifact management. They also developed a separate system for batch inference that integrates with their data warehouse, enabling large-scale text processing operations.

### Infrastructure and Training

The team worked on establishing GPU infrastructure in their Kubernetes environment, implementing:

• Karpenter for GPU node provisioning
• NVIDIA device plugin for GPU resource management
• Integration with HuggingFace transformers for model training
• Support for advanced techniques like LoRA fine-tuning
### Evaluation and Prompt Engineering

The platform includes specialized libraries for model evaluation and prompt engineering:

• Integration with HuggingFace's evaluate library
• Custom metrics development
• Template-based prompt generation
• Few-shot learning support with semantic similarity-based example selection
## Production Applications

The platform has enabled several production applications:

• Automatic Documentation: AI-powered documentation of data warehouse tables
• Ghostwriter: Automated documentation generation for care coordinator interactions
• Coverage Checker: First customer-facing GenAI implementation for insurance plan questions
• Clinical Scribe: Real-time visit transcription and medical documentation generation
• Records Collection: Automated medical information gathering and processing
• ChatIH: Internal chat interface for 400+ employees with specialized assistants
## Key Learnings and Best Practices

The case study highlights several important lessons for implementing LLMOps in a regulated environment:

### Flexibility and Modularity

• Maintaining adaptability in rapidly evolving technology landscape
• Building composable tools rather than monolithic solutions
• Enabling quick pivots to new priorities and technologies
### Open Source Integration

• Leveraging existing open-source tools where possible
• Using standard interfaces for better tool integration
• Building on established patterns like the OpenAI API specification
### Compliance and Security

• Early engagement with Legal and Security teams
• Careful handling of HIPAA-regulated data
• Structured review processes for new implementations
### Future Developments

The platform continues to evolve with new capabilities:

• Tool Calling and Agents: Development of infrastructure for LLM agents that can interact with internal tools and documentation
• RAG Implementation: Building unified API for retrieval-augmented generation capabilities
• Framework Integration: Exploring higher-level frameworks like LlamaIndex, CrewAI, and AutoGen
## Technical Implementation Details

The platform demonstrates sophisticated technical choices:

• Use of Kubernetes for infrastructure management
• Integration with multiple cloud providers
• MLFlow for model lifecycle management
• HuggingFace ecosystem integration
• Custom development of proxy services and client libraries
This case study represents a comprehensive approach to LLMOps in healthcare, showing how to balance innovation with regulatory compliance while maintaining scalability and usability. The platform's success is evidenced by its widespread adoption within the organization and the variety of production applications it supports.


