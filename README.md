# AI DevOps Demo

A demonstration project showcasing common DevOps issues and their fixes in an AI-powered application.

## 🚀 Quick Start

### Local Development
```bash
cd app
pip install -r requirements.txt
python app.py
```

### Docker
```bash
docker build -t ai-devops-demo .
docker run -p 5000:5000 ai-devops-demo
```

### Docker Compose
```bash
docker-compose up
```

### Kubernetes
```bash
kubectl apply -f k8s/
```

## 📁 Project Structure

```
ai-devops-demo/
├── app/                    # Flask application
│   ├── app.py             # Main application code
│   └── requirements.txt   # Python dependencies
├── Dockerfile             # Docker configuration (BROKEN)
├── docker-compose.yml     # Docker Compose setup (BROKEN)
├── k8s/                   # Kubernetes manifests
│   ├── deployment.yaml    # Deployment config (BROKEN)
│   └── service.yaml       # Service config
├── .github/workflows/     # CI/CD pipelines
│   └── ci.yml            # GitHub Actions (BROKEN)
├── logs/                  # Application logs
│   └── app.log           # Error logs for demo
├── commits.txt           # Bad commit messages
└── README.md             # This file
```

## 🔧 Issues to Fix

This project intentionally contains several DevOps issues that need to be addressed:

### Docker Issues
- Dockerfile has multiple security and best practice violations
- Docker Compose has incorrect port mappings and missing configurations

### Kubernetes Issues
- Deployment manifest is incomplete and insecure
- Missing resource limits and health checks

### CI/CD Issues
- GitHub Actions workflow is incomplete
- Missing testing, linting, and deployment steps

### Code Quality Issues
- Poor commit message practices
- Error logs indicating application problems

## 🎯 Learning Objectives

- Container security best practices
- Kubernetes resource management
- CI/CD pipeline development
- Application monitoring and logging
- Infrastructure as Code principles

## 📊 API Endpoints

- `GET /` - Welcome message
- `GET /health` - Health check
- `POST /predict` - AI prediction endpoint

## 🤖 AI Features

This demo includes a simulated AI prediction endpoint that demonstrates:
- Request/response handling
- Error management
- Logging integration
- API design patterns

## 📝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

MIT License - see LICENSE file for details