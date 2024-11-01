# Multi-modal RAG System for CFA Publications
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com/)
[![Apache Airflow](https://img.shields.io/badge/Apache%20Airflow-017CEE?style=for-the-badge&logo=apache-airflow&logoColor=white)](https://airflow.apache.org/)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)](https://aws.amazon.com)
[![Snowflake](https://img.shields.io/badge/Snowflake-29B5E8?style=for-the-badge&logo=snowflake&logoColor=white)](https://www.snowflake.com/)
[![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com)
[![Milvus](https://img.shields.io/badge/Milvus-00A4E4?style=for-the-badge&logo=milvus&logoColor=white)](https://milvus.io/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com)

WE ATTEST THAT WE HAVEN'T USED ANY OTHER STUDENTS' WORK IN OUR ASSIGNMENT AND ABIDE BY THE POLICIES LISTED IN THE STUDENT HANDBOOK
Contribution:
- a. Viswanath Raju Indukuri: 33%
- b. Snehal Shivaji Molavade: 33%
- c. Sai Vivekanand Reddy Vangala: 33%

## Individual Contributions

### Viswanath Raju Indukuri
- **Frontend Development**:
  - Created responsive Streamlit interface
  - Implemented document grid view and viewer
  - Developed user authentication UI
  - Designed interactive analysis tools

- **FastAPI Backend**:
  - Implemented secure endpoints
  - Developed Q&A functionality
  - Integrated JWT authentication

- **Report Generation**:
  - Implemented image integration
  - Designed report response

### Snehal Shivaji Molavade
- **Data Pipeline**:
  - Designed Airflow DAG architecture
  - Implemented web scraping

- **Storage Integration**:
  - Set up AWS S3 configuration
  - Implemented Snowflake integration

- **Multi-modal Processing**:
  - Implemented text extraction
  - Developed image processing
  - Created metadata management

### Sai Vivekanand Reddy Vangala
- **RAG Implementation**:
  - Set up llm model integration
  - Implemented vector db

- **Docker Configuration**:
  - Created containerization setup
  - Managed service orchestration

- **Documentation**:
  - Designed architecture diagrams
  - Managed project documentation

## Description
This project implements a comprehensive Multi-modal Retrieval Augmented Generation (RAG) system for CFA Institute Research Foundation Publications. The system automates the extraction of text and images from PDF files, stores them securely, and provides an interactive interface for users to explore and analyze the documents through various features like document summaries, Q&A capabilities, and report generation. By leveraging advanced AI technologies and cloud infrastructure, we create a seamless experience for accessing and analyzing financial research publications.

**Documentation**: [[Codelab Documentation Link]](https://codelabs-preview.appspot.com/?file_id=16rva6cQAW035xxCOuIZzpcxS_c5HmKfPp2t2TbLWZ6A#6)

**Demo Video Link**: [Video Link]

**Application URL**: http://viswanath.me:8501/

**Backend Service Link**: http://viswanath.me:8000/docs

**Data Processing Link**: http://localhost:8080/home

## Architecture Diagram:
![multi-modal_rag_system](https://github.com/user-attachments/assets/0efea28d-9969-48b4-8fb9-2073f7508273)



## About

### Problem Statement
The challenge we addressed was to create an intelligent system that could effectively process, analyze, and present CFA Institute's research publications. We needed to handle both text and visual content, implement retrieval mechanisms, and provide users with tools to interact with this knowledge base effectively.

### Scope
The project encompasses several key areas that work together to create a comprehensive solution:

The Data Ingestion Pipeline utilizes Apache Airflow to orchestrate the scraping and processing of CFA publications. This system automatically extracts text and images from documents, ensuring all content is properly captured and organized for further processing.

Our Storage Solution combines AWS S3 for document storage with Snowflake for metadata management. This dual-storage approach ensures that both structured and unstructured data are handled efficiently while maintaining quick access capabilities.

The Multi-modal RAG Implementation represents the core of our system. It processes both text and images intelligently, understanding the relationships between different content types and enabling sophisticated query responses. This system ensures that users receive contextually relevant information from their queries.

The User Interface provides an intuitive way to interact with the system. Through Streamlit, we've created a responsive frontend that allows users to explore documents, ask questions, and generate comprehensive reports. The interface is designed to be both powerful and easy to use.

The Backend Services, built with FastAPI, handle all the complex processing while ensuring security and performance. These services manage everything from user authentication to document analysis, providing a robust foundation for the entire system.

### Key Features

Our Data Processing capabilities are comprehensive and automated. The system handles document extraction, including both text and images, and processes this content to enable intelligent retrieval. The processed data is then stored securely and efficiently in snowflake and AWS.

The Document Analysis system is powered by llm models that understand both text and visual content. Users can generate summaries, ask questions, and receive answers that draw from the entire knowledge base. The system maintains context awareness, ensuring responses are relevant and accurate.

Our Report Generation feature creates professional documents that combine text and visual elements in the responses. These visual knowledge in reports make it easy to share insights from the analysis.

## Detailed System Overview

### 1. Data Acquisition and Processing
The system begins with automated data collection from CFA Institute Research Foundation Publications:

- **Web Scraping (Airflow DAG)**:
  - Extracts PDF files, titles, and summaries
  - Downloads images from publications
  - Processes metadata systematically

- **Storage Integration**:
  - AWS S3 buckets for PDFs and images
  - Snowflake database for structured metadata

### 2. Multi-modal RAG Implementation
Advanced RAG system combining text and image analysis:

- **Text Processing**:
  - Document chunking and indexing
  - Semantic understanding
  - Vector embeddings generation

- **Image Processing**:
  - Visual content extraction
  - Image-text alignment
  - Multi-modal context integration

- **RAG Components**:
  - OpenAI API/ NVIDIA with llama utilization
  - Vector DB management

### 3. Security and Authentication
Robust security measures protect user data and system access:

- **User Authentication**:
  - JWT-based authentication
  - Secure password handling
  - Session management

### 4. User Interface Features
Comprehensive interface for document interaction:

- **Document Selection**:
  - Grid view with thumbnails, titles

- **Document Viewer**:
  - PDF rendering
  - Image display
  - Text extraction view
  - Navigation controls

- **Analysis Tools**:
  - Interactive Q&A interface
  - Summary generation
  - Report creation

## Technical Details

### Data Flow
1. **Data Ingestion**:
```python
# Airflow DAG task for web scraping
def scrape_cfa_publications():
    # Web scraping logic
    page_content = get_page_content(url)
    publications = extract_publications(page_content)
    for pub in publications:
        process_publication(pub)
```

2. **Document Processing**:
```python
# PDF processing with PyMuPDF
def process_pdf(pdf_content):
    doc = fitz.open(stream=pdf_content, filetype="pdf")
    text_content = ""
    images = []
    for page in doc:
        text_content += page.get_text()
        images.extend(page.get_images())
    return text_content, images
```

3. **RAG Implementation**:
```python
# Multi-modal RAG query processing
async def process_query(query, context):
    # Initialize RAG components
    text_embeddings = generate_embeddings(query)
    relevant_chunks = retrieve_context(text_embeddings)
    
    # Generate response
    response = await generate_response(query, relevant_chunks)
    return response
```

### Storage Schema

1. **Snowflake Table Structure**:
```sql
CREATE TABLE publications (
    title STRING,
    brief_summary STRING,
    pdf_link STRING,
    image_link STRING,
    created_at TIMESTAMP_NTZ DEFAULT CURRENT_TIMESTAMP()
);
```

2. **Vector Store Configuration**:
```python
vector_store = MilvusVectorStore(
    host=MILVUS_HOST,
    port=MILVUS_PORT,
    dim=1024,
    collection_name="document_store"
)
```

## Project Structure
```.
├── Backend_FastAPIs
│   ├── Dockerfile
│   ├── __pycache__
│   └── main.py
├── Data_acquisition
│   ├── config
│   ├── dags
│   ├── docker-compose.yaml
│   ├── dockerfile
│   ├── logs
│   └── plugins
├── Frontend_Streamlit
│   ├── Dockerfile
│   └── app.py
├── LICENSE
├── Milvus
│   └── docker-compose.yml
├── Poc_files
│   ├── S3_test.py
│   ├── cfa_pdfs_images_s3.py
│   ├── cfa_pdfs_images_s3_csv.py
│   ├── cfa_pdfs_images_s3_sf.py
│   ├── cfa_pdfs_img_local.py
│   ├── cfa_pdfs_local.py
│   ├── cfa_pdfs_s3.py
│   ├── cfa_summary_local.py
│   ├── cfa_texts
│   ├── multimodal_report_generation (1).ipynb
│   ├── pdf-image_scrape.py
│   ├── pdf-image_scrape2.py
│   ├── publications_data.csv
│   ├── requirements.txt
│   └── snowflake_con_test.py
├── docker-compose.yml
└── requirements.txt
```

## Setup and Deployment

### Prerequisites
- Docker and Docker Compose v2.0+
- AWS Account with S3 access
- Snowflake Account with admin privileges
- OpenAI API Key
- NVIDIA API Key (optional)

1. Clone the repository to get all the source code on your machine 
 ```
 docker push Username/ImageNameForFastapi:latest
 ```
 + Push Streamlit:
 ```
 docker push Username/ImageNameForStreamlit:latest
 ```
## Deploy in GCP VM

7. GCP docker setup, create folder, create docker compose file, scp the .env and json file, pull the images, run docker compose.
 + Install Docker:
 ```
 sudo apt update
 sudo apt install -y docker.io
 ```
 + Install Docker Compose:
 ```
 sudo curl -L "https://github.com/docker/compose/releases/download/v2.21.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
 sudo chmod +x /usr/local/bin/docker-compose
 ```
 + Create a Directory for Your Project:
 ```
 mkdir ~/yourapp
 cd ~/yourapp
 ```
 + scp json file to myapp and .env
 ```
 gcloud compute scp --project YourProjectName --zone YourZone-f /path to your root dir/ServiceAccountJson Username@InstanceName:/PathInGCPToyourapp/ServiceAccountJson
 gcloud compute scp --project YourProject --zone YourZone-f /path to your root dir/.env Username@InstanceName:/PathInGCPToyourapp/.env
 ```
8. nano docker-compose.yml:
```
services:
  fastapi:
    image: Username/ImageNameForFastapi:latest  # Pull from Docker Hub
    container_name: YourFastapiContainer
    ports:
      - "8000:8000"
    env_file:
      - ./.env  # Pass the .env file located in the root directory at runtime
    volumes:
      - ./ServiceAccountJson:/app/ServiceAccountJson  # Mount the JSON file at runtime
    networks:
      - app-network

  streamlit:
    image: Username/ImageNameForStreamlit:latest  # Pull from Docker Hub
    container_name: YourStreamlitContainer
    ports:
      - "8501:8501"
    depends_on:
      - fastapi
    env_file:
      - ./.env  # Pass the .env file located in the root directory at runtime
    volumes:
      - ./ServiceAccountJson:/app/ServiceAccountJson  # Mount the JSON file at runtime
    networks:
      - app-network

networks:
  app-network:
    driver: bridge
```

9. Pull the Docker images and Start the containers:
```
sudo docker-compose pull
sudo docker-compose up -d
```
 
## Accessing Application via Cloud:
After deploying application through Cloud, you can use the application at url: http://viswanath.me:8501/
