# Architecture

## Prototype

The first release is a static browser application. Fictional demo records are stored in browser local storage and can be exported as CSV or JSON.

## Target Azure architecture

- Azure Container Apps for the frontend and API
- Azure Database for PostgreSQL for application records
- Azure Key Vault for secrets
- Azure Container Registry for versioned images
- Azure Monitor and Application Insights for observability
- Bicep for repeatable infrastructure
- Azure Pipelines for continuous integration and deployment

Development, staging, and production will use separate configuration and secrets. Production member data must never be copied into development or committed to Git.

