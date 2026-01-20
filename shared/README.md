# Shared Directory

This directory contains shared resources across all microservices:

## Libraries (`libs/`)
- Common utility functions
- Shared middleware
- Database connection helpers
- Authentication utilities

## Configurations (`configs/`)
- Environment-specific configs
- Database schemas
- API documentation templates

## Schemas (`schemas/`)
- Data validation schemas
- API request/response schemas
- Database table definitions

## Usage
```bash
# Install shared libraries
npm install --workspace=shared/libs

# Import in services
const { validateUser } = require('@shared/libs/validation');
```