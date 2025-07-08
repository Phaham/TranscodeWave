# TranscodeWave

A distributed video transcoding service built with RabbitMQ, GStreamer, and S3-compatible storage (e.g., MinIO), complemented by a React frontend and FastAPI backend.

## Overview

TranscodeWave orchestrates efficient, scalable video transcoding workflows:

- **RabbitMQ:** Queues and distributes transcoding tasks across worker nodes.  
- **GStreamer:** Performs media processing and format conversions.  
- **MinIO (S3-compatible):** Stores source and transcoded video files.  
- **FastAPI:** Exposes REST and WebSocket APIs for job control and monitoring.  
- **React:** Provides a user-friendly interface for submitting jobs and tracking progress.  

## Getting Started

### Prerequisites

- Docker & Docker Compose  
- Node.js & npm (for frontend)  

### Setup

1. **Clone the repo**  
   ```
   git clone https://github.com/phaham/TranscodeWave.git
   cd TranscodeWave

2. **Env file**
```
    S3_ENDPOINT_URL=http://minio:9000
    S3_ACCESS_KEY=your_access_key
    S3_SECRET_KEY=your_secret_key
    S3_BUCKET=your_bucket_name

3. ``` docker-compose up```

4. **Frontend**
```
cd frontend
npm install
npm start
```
