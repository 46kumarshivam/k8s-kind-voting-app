# K8s Kind Voting App

A comprehensive guide for setting up a local Kubernetes cluster using Kind, deploying a voting application, and configuring monitoring with Prometheus and Grafana.

## Overview

This guide covers the steps to:
Install Docker and Kind on a local machine.
Create a local Kubernetes cluster using Kind.
Install and access kubectl.
Deploy a voting application with multiple services (vote, result, Redis, database, worker).
Install and configure monitoring using Prometheus and Grafana via Helm charts.
Access dashboards to observe application metrics and application health.


## Architecture

![Architecture diagram](k8s-kind-voting-app.png)

## Observability

![Grafana diagram](grafana.png)
![Prometheus diagram](prometheus.png)

* A front-end web app in [Python](/vote) which lets you vote between two options
* A [Redis](https://hub.docker.com/_/redis/) which collects new votes
* A [.NET](/worker/) worker which consumes votes and stores them in…
* A [Postgres](https://hub.docker.com/_/postgres/) database backed by a Docker volume
* A [Node.js](/result) web app which shows the results of the voting in real time



Automated Deployment of Local Kubernetes Applications with Monitoring

Description:

Led the deployment of a scalable voting application on a local Kind Kubernetes cluster using Helm charts for monitoring with Prometheus and Grafana. Managed services, dashboards, and metrics for real-time observation and efficient resource utilization.

Key Technologies:

Kind for local Kubernetes cluster setup.
Docker for containerizing applications and services.
Helm for deploying Prometheus and Grafana stack.
Prometheus and Grafana for observability and monitoring.
Python, Node.js, .NET, Redis, and Postgres for core application functionality.
kubectl as CLI tool for Kubernetes management.

### Achievements:

Successfully deployed a multi-service voting application on a local Kind Kubernetes cluster.
Integrated Prometheus and Grafana dashboards for real-time monitoring.
Automated deployment using Helm charts for faster setup and testing.
Designed architecture for scalability, observability, and resilience in a local development environment.



