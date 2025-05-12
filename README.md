# Sequor Integrations

Production-ready, tested integrations for [Sequor](https://sequor.dev) – the SQL-centric, code-first platform for modern app/API integration.

## Overview

This repository contains pre-built integration flows for popular services including Salesforce, Shopify, Mailchimp, and many more. Each integration provides:

- **Production-ready implementation** with continuous testing and validation
- **Complete bidirectional data flows** for ingesting data and updating external systems
- **Pre-solved common challenges** including authentication, pagination, and response mapping
- **Consistently structured flows** following best practices for maintainability

## Integration Structure

Each integration follows a consistent pattern:

```
flows/
  └── <system_name>_<verb>_<object>.yaml  # Integration flow (e.g. mailchimp_fetch_subscribers.yaml)
  └── <system_name>_env.yaml                # Environment variables required for the integration
sources/
  └── <system_name>_*.yaml                  # Source configurations
```

## Environment Setup

Before running any integration flow:

1. Locate the relevant `<system_name>_env.yaml` file for your integration
2. Add the required environment variables to your Sequor environment
3. Run the desired integration flow

## Learning From Examples

Even if your target system isn't included, these integrations demonstrate reusable patterns for:

- Authentication flows (OAuth, API keys, etc.)
- Configuring and parameterizing HTTP requests
- Response parsing and database mapping
- Implementing pagination strategies
- Bidirectional data synchronization

The repository showcases approximately 10 common integration patterns that you can apply to build your own custom integrations.

## Getting Started

```bash
# Clone the repository
git clone https://github.com/sequor/sequor-integrations.git

# Navigate to the repository
cd sequor-integrations

# Configure environment variables
# (Add required values from <system_name>_env.yaml to your Sequor environment)

# Run an integration flow. For example:
sequor run flows/mailchimp_fetch_subscribers.yaml
```

## Contributing

We welcome contributions! If you've built an integration that others might find useful, please consider submitting a pull request.

## Stay Connected

We continuously add new integrations. Subscribe to the [Sequor newsletter](https://buttondown.com/sequor) to receive updates.


