Run Bizora's local PostgreSQL on Linux with Docker Compose
This guide shows you how to start, verify, reset and troubleshoot the local PostgreSQL database used for Bizora development. It also covers the Redis and WireMock services that run beside it.
Scope: local development only. The credentials in this guide are for your own machine. Never reuse them in cloud environments.
Authorship: drafted with AI assistance, then reviewed and tested by the author.
Tested on: <distribution and version, Docker version, date>
What you will set up
Service
Image
Host port
Purpose
postgres
postgres:16-alpine
5432
Application database (bizora_dev)
redis
redis:7-alpine
6379
Cache, sessions and rate limits (when implemented)
wiremock
wiremock/wiremock:3.9.1
8080
HTTP stubs for third-party callbacks and sandboxes