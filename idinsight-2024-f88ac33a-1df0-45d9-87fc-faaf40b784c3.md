# IDInsight: Optimizing Text-to-SQL Pipeline Using Agent Experiments (2024)

https://idinsight.github.io/tech-blog/blog/aam_pseudo_agent/

## Short Summary

Ask-a-Metric developed a WhatsApp-based AI data analyst that converts natural language questions to SQL queries. They evolved from a simple sequential pipeline to testing an agent-based approach using CrewAI, ultimately creating a hybrid "pseudo-agent" pipeline that combined the best aspects of both approaches. While the agent-based system achieved high accuracy, its high costs and slow response times led to the development of an optimized pipeline that maintained accuracy while reducing query response time to under 15 seconds and costs to less than $0.02 per query.

## Long Summary

# Ask-a-Metric: Evolution of a Production Text-to-SQL System

Ask-a-Metric is a WhatsApp-based AI data analyst system that enables natural language querying of SQL databases, specifically designed for the development sector. The project showcases a practical evolution of LLM deployment approaches, moving from a simple pipeline to an agent-based system, and finally to an optimized hybrid solution.

# Initial Simple Pipeline Implementation

• Built using Python's FastAPI framework
• Followed functional programming paradigm
• Designed for rapid deployment and quick feedback
• Encountered significant challenges:
# Agent-Based Approach Exploration

• Implemented using CrewAI framework
• System Architecture:
• Performance Metrics:
• Target Requirements:
# Optimization Insights from Agent Experiments

• Key Observations:
• Optimization Parameters:
• Used agent experiments as implicit parameter space search
# Final Pseudo-Agent Pipeline Implementation

## Architecture Improvements

• Object-oriented refactoring of codebase
• Modular components:
• Retained successful patterns from agent approach while eliminating overhead
## Technical Optimizations

• Task breakdown into smaller, focused steps
• Removed unnecessary agent operations:
• Data optimization:
• Purpose-built tools with specific scopes
## Performance Achievements

• Response time reduced to < 15 seconds
• Cost per query reduced to < $0.02
• Maintained high accuracy levels from agent-based approach
# Production Considerations and Future Development

## Current Focus Areas

• Continuous improvement of key metrics:
## Feature Development Pipeline

• Multi-turn chat capabilities
• Streamlined user onboarding
• Multi-language support
• Context-specific adaptations
## Deployment Strategy

• Testing in multiple contexts
• Pilot program feedback integration
• Focus on accessibility for social impact sector
• Emphasis on maintaining low costs while ensuring accuracy
# Technical Lessons Learned

• Agent-based systems can serve as excellent prototyping tools
• Hybrid approaches can combine benefits of different architectures
• Importance of modular design in LLM systems
• Value of systematic optimization in production deployments
• Balance between sophistication and practical constraints
The case study demonstrates a pragmatic approach to LLMOps, showing how different architectural approaches can be evaluated and combined to create an optimal production system. The evolution from a simple pipeline through agent-based experimentation to a hybrid solution provides valuable insights for similar LLM deployment projects.


