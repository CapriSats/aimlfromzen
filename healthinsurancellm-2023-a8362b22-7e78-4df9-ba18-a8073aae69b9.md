# HealthInsuranceLLM: Building an On-Premise Health Insurance Appeals Generation System (2023)

https://www.youtube.com/watch?v=lfoZPp6tLm4

## Short Summary

Development of an LLM-based system to help generate health insurance appeals, deployed on-premise with limited resources. The system uses fine-tuned models trained on publicly available medical review board data to generate appeals for insurance claim denials. The implementation includes Kubernetes deployment, GPU inference, and a Django frontend, all running on personal hardware with multiple internet providers for reliability.

## Long Summary

# Building an On-Premise Health Insurance Appeals Generator

## Project Overview

This case study details the development and deployment of an LLM-based system designed to generate health insurance appeals. The project addresses the significant challenge of health insurance claim denials in the American healthcare system, where insurers like Anthem Blue Cross deny approximately 20% of claims. The system was built with limited personal resources rather than enterprise-level infrastructure, demonstrating practical LLMOps implementation in a constrained environment.

## Data Collection and Processing

### Training Data Sources

• Primary source: California Independent Medical Review Board data
• Additional potential sources identified but not used:
### Synthetic Data Generation

• Used LLMs to generate synthetic training data
• Process:
• Challenges addressed:
## Model Development

### Fine-tuning Process

• Used Oxal for fine-tuning implementation
• Infrastructure:
• Cost efficiency:
## Infrastructure and Deployment

### Hardware Setup

• On-premise deployment using:
• Power considerations:
### Kubernetes Deployment

• Key deployment specifications:
• Deployment challenges:
### Frontend Implementation

• Django-based frontend choice:
### Network Infrastructure

• Autonomous system setup with three upstream providers
• Redundancy and reliability considerations
• Hurricane Electric Fremont 2 connectivity
## Technical Challenges and Solutions

### GPU Optimization

• Single GPU inference approach
• Fine-tuning optimization:
### System Limitations

• CPU inference challenges:
• Batch processing:
### Deployment Challenges

• Hardware reliability issues
• Container management:
## Production Considerations

### Performance Optimization

• GPU utilization monitoring
• Temperature and power consumption management
• Batch size optimization potential for multiple users
### Reliability Engineering

• Multiple internet provider setup
• Hardware redundancy planning
• System recovery procedures
### Future Improvements

• Potential Intel-specific accelerator integration
• Scaling considerations for multiple users
• Enhanced model evaluation and testing
## Lessons Learned

### Infrastructure Design

• Importance of hardware selection and compatibility
• Power management in constrained environments
• Network redundancy requirements
### Model Deployment

• Container version pinning necessity
• Resource allocation optimization
• Hardware-software compatibility considerations
### System Architecture

• Benefits of modular design
• Importance of monitoring and logging
• Scaling considerations for future growth

