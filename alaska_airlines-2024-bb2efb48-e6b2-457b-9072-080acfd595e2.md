# Alaska Airlines: AI-Powered Natural Language Flight Search Implementation (2024)

https://www.youtube.com/watch?v=I4DTkOBeZ30&t=829s

## Short Summary

Alaska Airlines implemented a natural language destination search system powered by Google Cloud's Gemini LLM to transform their flight booking experience. The system moves beyond traditional flight search by allowing customers to describe their desired travel experience in natural language, considering multiple constraints and preferences simultaneously. The solution integrates Gemini with Alaska Airlines' existing flight data and customer information, ensuring recommendations are grounded in actual available flights and pricing.

## Long Summary

# Alaska Airlines Natural Language Flight Search Implementation

## Company Background and Context

Alaska Airlines, the fifth-largest US airline serving 45 million customers annually, has demonstrated a strong commitment to digital innovation and AI implementation. The company has previously established a real-time data foundation connecting guest data with operations data, laying the groundwork for more sophisticated AI applications.

## AI Strategy and Implementation Approach

• Developed an 8-step process from idea selection to production deployment
• Adopted a multi-model approach rather than relying on a single AI solution
• Started with internal-facing opportunities before moving to customer-facing applications
• Maintained strong focus on maintaining customer trust and care in AI implementations
## Technical Architecture and Integration

### Core Infrastructure

• Modernized tech stack from monolithic to microservices-based cloud-native solutions
• Built on existing Google Cloud infrastructure including:
### Gemini Implementation

• Primary use case: Natural Language Destination Search
• Key technical components:
### Data Integration Points

• Customer profile data
• Flight availability and pricing
• Destination information
• Historical booking patterns
• Real-time inventory
## Development Process and Methodology

• Rapid prototyping and iteration based on customer feedback
• Initially started with chatbot approach but pivoted based on user preference for immersive experience
• Development from concept to production in matter of weeks
• Strong emphasis on testing and validation before customer-facing deployment
## Production Considerations

### Quality and Safety Measures

• Implementation of factuality checks through function calling
• Verification of flight availability before making recommendations
• Price validation in real-time
• Multi-language support validation
### User Experience Design

• Focus on natural conversation rather than traditional search parameters
• Integration of visual elements (maps, images) for improved user experience
• Dynamic content generation tailored to user queries
• Support for complex multi-constraint queries
## Technical Challenges and Solutions

• Ensuring real-time availability of flight data
• Managing multiple constraint satisfaction in search queries
• Integrating multiple data sources seamlessly
• Maintaining system performance at scale
• Handling multiple languages and cultural contexts
## Production Infrastructure

### Core Components

• Microservices architecture
• Cloud-native deployment
• API integration layer
• Customer data platform
• Machine learning recommendation system
### Integration Points

• Google Cloud Platform services
• Existing airline booking systems
• Customer database
• Pricing systems
• Maps and location services
## Monitoring and Maintenance

• Real-time verification of recommendations
• Price accuracy monitoring
• Language quality assurance
• System performance metrics
• User interaction tracking
## Results and Impact

• Successfully launched first customer-facing AI travel search capability
• Improved customer experience through natural language interaction
• Enhanced ability to handle complex travel queries
• Support for multiple languages and cultural contexts
• Integration with existing airline systems and data
## Future Development Plans

• Expansion of use cases beyond initial search functionality
• Integration with additional customer service touchpoints
• Enhanced personalization capabilities
• Broader language support
• Integration with merged airline systems (pending Hawaiian Airlines merger)
## Key Learnings

• Importance of starting with internal applications before customer-facing ones
• Value of rapid prototyping and customer feedback
• Need for strong data infrastructure before AI implementation
• Importance of maintaining trust while innovating
• Benefits of multi-model approach to AI implementation
## Production Best Practices

• Maintain strong focus on factuality and accuracy
• Ensure real-time validation of recommendations
• Integrate closely with existing systems
• Build on solid data infrastructure
• Prioritize user experience over technical sophistication
• Implement robust testing and validation processes
• Maintain flexibility for future expansion

