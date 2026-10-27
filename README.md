# InsureFlow

InsureFlow is a prototype insurance claims platform built as a set of
microservices. Claims are processed automatically by three rule-based
agents (Coverage, Evidence, Decision). Risky or incomplete cases are
always sent to a human reviewer.

> ⚠️ Prototype with fictional data only. It is not intended for real claims.

This repository contains the project documentation, the architecture
diagrams and links to all service repositories.

## Services

| Service | Responsibility |
|---|---|
| [claims-service](../claims-service) | Claims, statuses, decisions |
| [policies-service](../policies-service) | Policies and coverage checks |
| [documents-service](../documents-service) | Evidence and metadata |
| [agents-service](../agents-service) | Orchestration of the 3 agents |
| [risk-service](../risk-service) | Risk score (0-100) |
| [reviews-service](../reviews-service) | Mandatory human review |

## Tech stack
REST + Swagger · RabbitMQ (AMQP) · PostgreSQL · Docker Compose · Kubernetes (kind)

## Team
Sandi Cejan · Kristjan Brataševec · Maksimilian Bertoncelj, group 3 (ZavarovalnicaOrg)