# NICE: Natural Language to SQL System with Production Safeguards for Contact Center Analytics (2024)

https://www.youtube.com/watch?v=Qb3GIIq-qGs

## Short Summary

NICE implemented a system that allows users to query contact center metadata using natural language, which gets translated to SQL queries. The solution achieves 86% accuracy and includes critical production safeguards like tenant isolation, default time frames, data visualization, and context management for follow-up questions. The system also provides detailed explanations of query interpretations and results to users.

## Long Summary

# Natural Language to SQL System for Contact Center Analytics at NICE

## Overview

NICE developed a production system that enables users to query contact center metadata using natural language, which is then converted to SQL queries. The system is designed with multiple safeguards and features to ensure reliable operation in a production environment, moving beyond simple demo implementations to address real-world challenges.

## Core Architecture

• Basic flow involves:
## Production Safeguards and Features

### Metadata Management

• Implemented translation table for column names
• Allows for schema changes without LLM retraining
• Handles special cases like behavioral scores where higher values might indicate worse performance
• Provides context about data meaning to LLM for accurate query generation
### Security Implementation

• Strict tenant isolation
• Database access control handled separately from LLM system
### Query Parameter Management

• Handles imprecise user queries through defaults
• Implements automatic limitations:
• Time frame handling:
### Result Presentation and Interpretation

• Multiple visualization options:
• Uses LLM to determine optimal visualization method
• Provides text descriptions of results including:
• Explicit clarification of potentially ambiguous interpretations
### Follow-up Question Handling

• Maintains context between queries
• Stores previous SQL queries for context
• Approach to context management:
• Handles query refinements effectively:
### Data Refresh Strategy

• Caches SQL queries for repeated execution
• Enables consistent daily updates without LLM regeneration
• Reduces risk of inconsistent results from multiple LLM generations
### Error Prevention and Handling

• Validates queries against business rules
• Prevents inappropriate or out-of-scope questions
• System provides clear feedback when:
## Technical Implementation Details

• Achieves 86% accuracy in query translation
• Built on public database with 10,000 questions and 200 database schemas
• Handles complex multi-table queries
• Supports various visualization types
• Implements robust context management system
## Challenges and Solutions

• Query Precision:
• Result Interpretation:
• Follow-up Questions:
## Best Practices Identified

• Always provide explicit explanation of query interpretation
• Implement strong security boundaries
• Use default parameters for common scenarios
• Cache and reuse successful queries
• Provide multiple visualization options
• Include clear data interpretation guidelines
• Maintain conversation context appropriately
• Handle imprecise queries gracefully
• Implement robust error handling

