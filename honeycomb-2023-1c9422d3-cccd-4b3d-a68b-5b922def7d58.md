# Honeycomb: Building and Scaling an LLM-Powered Query Assistant in Production (2023)

https://www.honeycomb.io/blog/we-shipped-ai-product

## Short Summary

Honeycomb implemented a Query Assistant powered by LLMs to help users better understand and utilize their observability platform's querying capabilities. The feature was developed rapidly with a "ship to learn" mindset, using GPT-3.5 Turbo and text embeddings. While the initial adoption varied across pricing tiers (82% Enterprise/Pro, 75% Self-Serve, 39% Free) and some metrics didn't meet expectations, it achieved significant successes: teams using Query Assistant showed 26.5% retention in manual querying vs 4.5% for non-users, higher complex query creation (33% vs 15.7%), and increased board creation (11% vs 3.6%). Notably, the implementation proved extremely cost-effective at around $30/month in OpenAI costs, demonstrated strong integration with existing workflows, and revealed unexpected user behaviors like handling DSL expressions and trace IDs. The project validated Honeycomb's approach to AI integration while providing valuable insights for future AI features.

## Long Summary

# Notes on Honeycomb's LLM Implementation Case Study

## Company/Use Case Overview

• Honeycomb: Observability platform facing user adoption challenges with complex querying
• Goal: Improve user experience and reduce learning curve for querying capabilities
• Solution: Query Assistant powered by LLMs to help users formulate queries
• Target: All users, with particular focus on new and free tier users
## Technical Implementation

### Architecture

• Primary models: GPT-3.5-turbo and text-embedding-ada-002
• Redis cluster for embedding vector storage
• Input tokens: ~1800 per request
• Response tokens: ~100 per request
### Operational Metrics

• Average monthly OpenAI cost: $30
• Redis node cost: ~$100 per node
• Latency stats:
### Cost Optimization Strategies

• Limited output token generation
• Optimized prompt engineering
• Used GPT-3.5 over GPT-4
• Focused on minimal but effective responses
## Success Metrics & Results

### Adoption Rates

• Enterprise/Pro Plus: 82% usage
• Self Serve: 75% usage
• Free tier: 39% usage
### User Behavior Metrics

• Manual query retention (week 6):
• Complex query creation:
• Board creation:
### Usage Patterns

• High initial usage dropping after first week
• Consistent usage for exploring new datasets
• Valuable for team onboarding
• Users "graduating" to manual querying
## Key Learnings & Insights

### Unexpected User Behaviors

• Successfully handled DSL expressions
• Processed trace ID lookups
• Adapted to query modifications
• Handled pseudo-SQL inputs
### Technical Insights

• Importance of rapid iteration
• Value of production data for improvements
• Need for comprehensive monitoring
• Benefits of structured user feedback
### Implementation Strategy

• "Ship to learn" approach
• Rapid iteration based on user feedback
• Focus on user behavior analysis
• Continuous performance monitoring
## Business Impact

### Positive Outcomes

• Improved user onboarding
• Enhanced product accessibility
• Cost-effective implementation
• Stronger user engagement
### Areas for Improvement

• Free tier adoption rates
• Feature discovery
• Long-term retention patterns
• Trigger creation correlation
## Future Directions

### Potential Improvements

• Enhanced feature discovery
• Expanded use cases
• Integration with other product areas
• Improved onboarding flows
### Considerations

• Model selection and upgrades
• Cost vs. performance balance
• User experience optimization
• Feature discoverability
## Key Takeaways

### Success Factors

• Low implementation cost
• Strong correlation with key metrics
• Positive user feedback
• Effective onboarding tool
### Challenges Addressed

• Complex learning curve
• User adoption barriers
• Query formulation difficulty
• Technical implementation complexities

