# Backend Service

The logs-gateway service is responsible for user related operations:

- expose two endpoints to get logs: Rest and gRPC
- stream logs to kafka
- the logs-gateway service checks the validity of the jwt token through :
  - jwt signature verification
  - a cached list of invalid tokens (blacklist topic)
