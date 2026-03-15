## Project 3: Log Monitoring & Observability System

**File:** `README.md`

```markdown
# Log Monitoring & Observability (ELK Stack)

A centralized logging solution designed to monitor containerized applications and provide real-time visual insights into system health.

## 📊 Stack Components


- **Elasticsearch:** Search and analytics engine.
- **Logstash:** Server-side data processing pipeline.
- **Kibana:** Data visualization dashboard.
- **Docker Compose:** Orchestration of the ELK stack.

## 🔍 Implementation Details
- **Log Collection:** Logstash collects logs from multiple Docker containers.
- **Filtering:** Custom Grok filters to parse application logs into structured data.
- **Visualization:** A Kibana dashboard showing:
    - 404/500 Error rates.
    - Traffic volume over time.
    - Geographic distribution of requests.

## 🏃 How to Run
1. Clone the repo.
2. Ensure Docker and Docker Compose are installed.
3. Run the stack:
   ```bash
   docker-compose up -d
