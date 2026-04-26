# Bud Financial / Scotts Miracle-Gro: Building Personalized Financial and Gardening Experiences with LLMs (2024)

https://www.youtube.com/watch?v=O2xVgbSGqwc

## Short Summary

This case study explores how Bud Financial and Scotts Miracle-Gro leverage Google Cloud's AI capabilities to create personalized customer experiences. Bud Financial developed a conversational AI solution for personalized banking interactions, while Scotts Miracle-Gro implemented an AI assistant called MyScotty for gardening advice and product recommendations. Both companies utilize various Google Cloud services including Vertex AI, GKE, and AI Search to deliver contextual, regulated, and accurate responses to their customers.

## Long Summary

# Building Personalized Customer Experiences with LLMs at Bud Financial and Scotts Miracle-Gro

## Overview

This case study examines how two distinct companies - Bud Financial in the banking sector and Scotts Miracle-Gro in the gardening industry - are implementing LLMs and AI technologies to create personalized customer experiences. Both companies leverage Google Cloud's infrastructure and AI services to deliver contextual, accurate, and regulated responses to their customers.

## Bud Financial's Implementation

### Business Context

• Bud Financial works with banks and fintech companies to help them understand customers through transactional data
• Focus on delivering personalized experiences in a highly regulated financial environment
• Developed "YS" solution for in-app customer interactions
### Technical Architecture

• Models trained from scratch in offline data environment
• Infrastructure running on Google Kubernetes Engine (GKE)
• Utilizes mix of TPUs, GPUs, and Intel compute-optimized machine types
• Implementation focuses on:
• Uses Gemini through Vertex AI API suite
• Started with Google's JAP Builder (now Vertex Conversation)
### MLOps Considerations

• Heavy focus on explainability and transparency
• Model training specifically designed for transactional data understanding
• Implementation of deterministic journeys for regulatory compliance
• Comprehensive testing approach:
• User feedback analysis and monitoring
## Scotts Miracle-Gro Implementation

### Business Context

• Developed MyScotty AI assistant for gardening advice and product recommendations
• Focus on providing personalized gardening experiences
• Handles multimodal interactions including image recognition for plants
### Technical Stack

• Built entirely on Google Cloud
• Key components:
### MLOps Challenges and Solutions

### Product Recommendation System

• Unique approach different from traditional e-commerce recommendations
• Requires highly specific and contextualized recommendations
• Implementation considerations:
### Knowledge Management

• Handles large volumes of unstructured data from research and SMEs
• Challenges in unstructured data governance
• Solutions include:
• Focus on accuracy and currency of information
### Search Implementation

• Vertex AI Search implementation for natural language queries
• Features:
## Production Considerations

### Testing and Validation

• Sandbox testing for risk management
• Internal validation before public deployment
• Continuous monitoring of response accuracy
### Performance Metrics

• Focus on user feedback
• Trust and engagement metrics
• Response relevance tracking
• Personalization effectiveness measurement
### Integration and Deployment

• Seamless integration with Google Cloud services
• Automated scaling and infrastructure management
• Regular updates and improvements based on user interaction
## Results and Impact

### Bud Financial

• Improved customer trust through personalized interactions
• Double response rate for personalized messages
• Enhanced regulatory compliance while maintaining personalization
### Scotts Miracle-Gro

• Accelerated development of personalized products
• Improved customer communication
• More relevant and contextual product recommendations
• Enhanced gardening advice delivery

