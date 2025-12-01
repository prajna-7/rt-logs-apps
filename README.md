# rt-logs-apps
This repo is part of a portfolio project to demonstrate real-time log processing on AWS.

Application repository for the **Real-Time Log Processing Platform on AWS**.

This repo contains Python microservices and load testing code that will generate
logs and metrics for the platform. The services will run on Amazon EKS and send
logs to a centralized logging pipeline (Fluent Bit → Kafka → Logstash →
OpenSearch/Elasticsearch → Kibana).

## Structure

- `payments-service/` – Sample microservice that simulates payment operations and emits logs/metrics.
- `orders-service/` – Sample microservice that simulates order management and emits logs/metrics.
- `locust/` – Load testing scenarios using Locust, to generate traffic and logs.
- `.github/workflows/` – GitHub Actions CI workflows (tests, linting, security scans, builds).

## Next steps (future phases)

- Add Python applications for `payments-service` and `orders-service`.
- Add Dockerfiles and CI workflows for building and scanning images.
- Deploy these services to Amazon EKS as part of the overall logging platform.
