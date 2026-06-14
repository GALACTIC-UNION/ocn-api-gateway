# OCN API Gateway
**[OCN - CORE INTEGRATION]** Unified external API surface for the Omniscient Civilization Nexus.

## Overview
Single entry point for all external integrations, operator tooling, and cross-domain API calls. Handles authentication, rate limiting, request routing, schema validation, and API versioning across all 9 OCN domains.

## Features
- OpenAPI 3.1 specification for all domains
- JWT + quantum-signed token authentication
- Per-domain and per-operator rate limiting
- Automatic circuit-breaking and fallback routing
- Full request/response audit logging to Enforcement Ledger

## Structure
```
src/
├── router/            # Request routing and load balancing
├── auth/              # Authentication and authorization
├── rate-limiting/     # Adaptive rate limiting engine
├── validation/        # Schema and Accord-compliance validation
├── logging/           # Audit log pipeline
└── api/               # Gateway management API
config/
├── routes.yaml
├── auth-policy.yaml
├── rate-limits.yaml
└── circuit-breakers.yaml
docs/
├── api-reference.md
└── integration-guide.md
openapi/
└── ocn-api-v1.yaml    # Full OpenAPI 3.1 specification
```

## License
Apache 2.0
