# Ghostwriter: Building an AI-Powered Email Writing Assistant with Personalized Style Matching (2024)

https://www.youtube.com/watch?v=9B-BiKH_xjg

## Short Summary

Shortwave developed Ghostwriter, an AI writing feature that helps users compose emails that match their personal writing style. The system uses embedding-based semantic search to find relevant past emails, combines them with system prompts and custom instructions, and uses fine-tuned LLMs to generate contextually appropriate suggestions. The solution addresses two key challenges: making AI-generated text sound authentic to each user's style and incorporating accurate, relevant information from their email history.

## Long Summary

# Building Ghostwriter: An AI Email Writing Assistant at Shortwave

## Overview

Shortwave is developing an advanced email client that integrates AI capabilities to enhance the email experience. Their Ghostwriter feature, launched in the previous year, focuses on AI-powered email composition that matches each user's writing style. The system was later expanded to include real-time autocompletion capabilities.

## Technical Architecture

### Data Processing Pipeline

• Email content preprocessing and cleaning pipeline to extract clean text from complex email threads
• Embedding generation for all user emails using vector embeddings
• Storage of embeddings in a vector database for quick retrieval
• Real-time semantic search capabilities to find relevant previous emails
### Core Components

• Vector database for storing and searching email embeddings
• Embedding model for converting emails to vector representations
• Fine-tuned LLM for text generation (based on GPT-4)
• Custom prompt engineering system
• Email cleaning and preprocessing pipeline
### System Flow

• Offline Processing:
• Real-time Generation:
## Key Technical Challenges and Solutions

### Style Matching

• Initial Approach: Providing psychological profile of user's writing style
• Fine-tuning Approach:
### Information Accuracy

• Vector search to find relevant past emails containing similar information
• Integration with AI search feature for fact lookups
• Training examples crafted for specific scenarios (WiFi passwords, addresses)
• No-hallucination examples included in training data
### Output Formatting

• Fine-tuning helped solve specific formatting challenges:
## Production Considerations

### Safety and Security

• Strict "no actions without user confirmation" policy
• All AI suggestions require explicit user approval
• System designed to prevent automatic sending of sensitive information
### Data Pipeline

• Robust email cleaning pipeline to handle nested threads
• Extraction of clean text content from complex email structures
• Careful handling of training data generation
### Model Management

• Flexible architecture allowing easy model swapping
• Support for multiple embedding models
• Ability to gradually roll out new models to users
## Future Improvements

### Model Enhancement

• Exploring per-user fine-tuning as costs decrease
• Planning for more diverse training examples
• Investigation of newer language models
• Incorporation of user feedback into training
### Content Relevance

• Improving ranking for similar emails
• Exploring cross-encoding techniques
• Development of fine-grained snippet selection
• Testing multiple embedding models per email
### Infrastructure

• Continued improvement of data cleaning pipeline
• Better handling of messy email data
• Enhanced training data synthesis
## Results and Impact

• Successfully deployed in production
• Positive user adoption of writing features
• System capable of maintaining personal writing style while incorporating relevant information
• Demonstrated ability to handle complex email contexts and formatting requirements
## Technical Implementation Details

### Training Data Generation

• Synthetic data created from real email patterns
• Random cursor position simulation
• Specific examples for fact lookup scenarios
• Careful balance of completion vs. no-completion cases
### System Integration

• Integration with Gmail API
• Real-time processing capabilities
• Vector database optimization for quick retrieval
• Careful handling of email threading and formatting

