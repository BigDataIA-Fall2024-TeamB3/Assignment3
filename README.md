# Multimodal RAG System for CFA Publications

[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apache-airflow&logoColor=white)](https://airflow.apache.org/)
[![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)](https://aws.amazon.com)
[![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)](https://www.snowflake.com/)
[![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![NVIDIA](https://img.shields.io/badge/NVIDIA-76B900?style=for-the-badge&logo=nvidia&logoColor=white)](https://www.nvidia.com/)
[![LlamaIndex](https://img.shields.io/badge/LlamaIndex-000000?style=for-the-badge&logo=llama&logoColor=white)](https://llamaindex.ai/)
[![Milvus](https://img.shields.io/badge/Milvus-00A4FF?style=for-the-badge&logo=milvus&logoColor=white)](https://milvus.io/)

WE ATTEST THAT WE HAVEN'T USED ANY OTHER STUDENTS' WORK IN OUR ASSIGNMENT AND ABIDE BY THE POLICIES LISTED IN THE STUDENT HANDBOOK

## Team Members and Contributions

### Member 1 (33%) - Backend Development and RAG Implementation
- Designed and developed the FastAPI backend architecture
- Implemented the RAG system using LlamaIndex and NVIDIA services
- Created the JWT authentication system
- Developed API endpoints for document processing and analysis
- Integrated vector store functionality using Milvus

### Member 2 (33%) - Frontend Development and User Experience
- Created the Streamlit frontend interface
- Designed the document viewer and chat interface
- Implemented real-time response streaming
- Developed the report generation interface
- Created user authentication flows and error handling

### Member 3 (33%) - Infrastructure and Data Pipeline
- Set up the Airflow pipeline for data collection
- Implemented AWS S3 and Snowflake integration
- Created Docker containerization setup
- Managed cloud infrastructure and deployment
- Developed the data processing pipeline

## Project Overview

The Multimodal RAG System for CFA Publications represents a sophisticated approach to document processing and analysis, specifically designed for handling CFA Institute Research Foundation Publications. This system combines advanced natural language processing, computer vision, and machine learning techniques to provide a comprehensive solution for document understanding and interaction.

### Core Capabilities

#### 1. Automated Data Collection
- Systematic scraping of CFA publications using Airflow and Selenium
- Intelligent document classification and categorization
- Automated metadata extraction and storage
- Real-time updates and synchronization

#### 2. Document Processing
- Advanced PDF text extraction with PyMuPDF
- Intelligent document chunking for optimal processing
- Image and table detection with computer vision
- Multi-format support including text, images, and tables

#### 3. RAG Implementation
- Context-aware document retrieval
- Hybrid search combining semantic and keyword approaches
- Source attribution and relevance scoring
- Dynamic prompt generation and optimization

#### 4. User Interface
- Intuitive document navigation and selection
- Real-time chat interface with streaming responses
- Interactive document viewer with highlighting
- Custom report generation capabilities

## System Architecture Diagram:
![multi-modal_rag_system](https://github.com/user-attachments/assets/b7c6c2be-84ba-4eff-bf96-4d6611169a37)


### 1. Data Ingestion Layer

#### Web Scraping Component
- Automated scheduling with Airflow
- Intelligent crawling of CFA website
- Document download and verification
- Error handling and retry mechanisms

#### Storage Management
- AWS S3 for document storage
- Snowflake for structured data and metadata
- Efficient data organization and retrieval
- Backup and versioning support

### 2. Processing Layer

#### Document Processing Pipeline
- Text extraction and normalization
- Image and table processing
- Metadata extraction and enrichment
- Quality assurance checks

#### Vector Processing
- Document embedding generation
- Milvus vector store integration
- Similarity search optimization
- Index management and updates

### 3. Presentation Layer

#### Frontend Components
- Responsive document grid view
- Interactive chat interface
- Document preview and navigation
- Progress indicators and notifications

#### User Management
- Secure authentication flow
- Session management
- Role-based access control
- User preferences handling

## Security Features

### Authentication System
- JWT-based authentication
- Secure password hashing with bcrypt
- Token refresh mechanism
- Session timeout handling

### Data Protection
- Encrypted data storage
- Secure file handling
- Access control mechanisms
- Audit logging

## Performance Optimizations

### Vector Search
- Optimized index structures
- Caching mechanisms
- Batch processing
- Query optimization

### Response Generation
- Streaming response handling
- Concurrent processing
- Resource management
- Load balancing

## Setup Instructions

### Prerequisites
1. Docker and Docker Compose installation
2. AWS account with appropriate permissions
3. Snowflake account setup
4. NVIDIA and OpenAI API keys
5. Python 3.9 or higher

### Environment Configuration
1. AWS credentials configuration
2. Snowflake connection setup
3. API key management
4. Environment variable configuration

### Installation Steps
1. Repository cloning and setup
2. Dependencies installation
3. Database initialization
4. Service configuration

### Deployment
1. Docker container building
2. Service orchestration
3. Environment verification
4. System health checks

## Usage Guide

### Document Management
1. Uploading and processing documents
2. Managing document metadata
3. Organizing document collections
4. Searching and filtering

### Query Interface
1. Formulating effective queries
2. Understanding response formats
3. Managing conversation context
4. Utilizing advanced features

### Report Generation
1. Creating custom reports
2. Including multimodal content
3. Formatting and styling
4. Exporting and sharing

## Error Handling and Recovery

### System Monitoring
- Health check implementation
- Error logging and tracking
- Performance monitoring
- Alert systems

### Recovery Procedures
- Automatic retry mechanisms
- Fallback strategies
- Data consistency checks
- System state recovery

## Future Enhancements

### Planned Features
1. Advanced visualization capabilities
2. Enhanced multimodal processing
3. Improved search algorithms
4. Extended API functionality

### Scalability Improvements
1. Distributed processing
2. Enhanced caching
3. Performance optimization
4. Resource management

## Support and Maintenance

### Documentation
- API documentation
- User guides
- Troubleshooting guides
- Best practices

### Support Channels
- Issue tracking
- Support tickets
- Documentation updates
- Community engagement

This comprehensive system provides a robust solution for processing and analyzing CFA publications, combining advanced technologies with user-friendly interfaces to deliver an efficient and effective document analysis platform.
