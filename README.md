# Trading Platform - Microservices Architecture

## Overview
A comprehensive trading platform built with microservices architecture, featuring authentication, order management, portfolio tracking, and administrative capabilities.

## Architecture
- **Auth Service**: JWT-based authentication and authorization
- **Order Service**: Order creation, management, and execution
- **Portfolio Service**: Portfolio tracking and analytics
- **Admin Service**: Administrative dashboard and user management
- **Order Worker**: Background job processing for order execution

## Technology Stack
- **Backend**: Node.js/Java Spring Boot
- **Database**: PostgreSQL/MongoDB
- **Message Queue**: Redis/RabbitMQ
- **Container**: Docker
- **Orchestration**: Kubernetes (EKS)
- **CI/CD**: Jenkins, ArgoCD
- **Monitoring**: Grafana, Prometheus
- **Security**: SonarQube, Trivy
- **Infrastructure**: Terraform, AWS

## Getting Started
```bash
# Clone repository
git clone <repository-url>

# Start local development
docker-compose up -d

# Run individual service
cd services/auth-service
npm install
npm start
```

## Services

### Auth Service
- Port: 3001
- Database: PostgreSQL
- Features: JWT authentication, user management

### Order Service  
- Port: 3002
- Database: PostgreSQL
- Features: Order CRUD, order validation

### Portfolio Service
- Port: 3003
- Database: MongoDB
- Features: Portfolio tracking, analytics

### Admin Service
- Port: 3004
- Database: PostgreSQL
- Features: User management, system monitoring

### Order Worker
- Queue: Redis
- Features: Background order processing

## Development

### Prerequisites
- Node.js 18+
- Docker & Docker Compose
- kubectl
- terraform

### Local Setup
1. Copy environment files: `cp .env.example .env`
2. Start dependencies: `docker-compose up -d postgres redis mongodb`
3. Run services: `npm run dev`

## Deployment

### Staging
```bash
kubectl apply -f infrastructure/k8s/overlays/staging/
```

### Production
```bash
kubectl apply -f infrastructure/k8s/overlays/production/
```

## Monitoring
- Grafana: http://localhost:3000
- Prometheus: http://localhost:9090
- Jaeger: http://localhost:16686

## Contributing
1. Create feature branch
2. Make changes
3. Run tests: `npm test`
4. Submit PR

## License
MIT# trading-platform
