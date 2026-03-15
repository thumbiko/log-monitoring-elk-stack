# 📊 Log Monitoring & Observability System (ELK Stack)

Real-time monitoring and log aggregation system for containerized microservices using the **Elasticsearch, Logstash, and Kibana (ELK)** stack.

## 🔎 Why this matters
In a DevOps environment, visibility is king. This project provides a centralized dashboard to track application errors and system performance in real-time.

## 🏗️ The Stack
- **Elasticsearch:** Distributed search engine for log storage.
- **Logstash:** Data processing pipeline to ingest and parse logs.
- **Kibana:** Visualization layer for creating NOC-style dashboards.
- **Filebeat:** Lightweight shipper for forwarding logs from containers.

## 📈 Dashboard Features
- **Error Tracking:** Visualization of 4xx and 5xx HTTP status codes.
- **Latency Monitoring:** Heatmap of request response times.
- **Resource Usage:** Tracking CPU/RAM spikes across Docker containers.

## 🚀 Setup
1. Clone the repository.
2. Run `docker-compose up -d`.
3. Navigate to `localhost:5601` to view the Kibana UI.
4. Logs from the sample `app` container will begin streaming automatically.

## 🛠️ DevOps Skills
- Log Aggregation & Parsing (Grok filters).
- Container Orchestration (Docker Compose).
- Operational Observability & Alerting.
