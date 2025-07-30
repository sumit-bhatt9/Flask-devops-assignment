
### 📄 `README.md`

```markdown
# Flask DevOps Assignment

This project demonstrates a complete CI/CD deployment pipeline for a Flask web application using:

- Docker
- GitHub Actions
- Kubernetes (via Minikube)

## 🔧 Tech Stack

- Python + Flask
- Docker
- GitHub Actions
- Kubernetes (Minikube)
- YAML (for K8s deployments)

## 🚀 Features

- Dockerized Flask app
- GitHub Actions pipeline for CI/CD
- K8s deployment with `Deployment` and `Service` manifests
- Live testing on Minikube

## 📂 Project Structure


.
├── app/
│   └── main.py
├── Dockerfile
├── k8s/
│   ├── deployment.yaml
│   └── service.yaml
├── .github/workflows/
│   └── main.yml
├── .gitignore
└── README.md

````

## 🐳 Docker

Build & run:
```bash
docker build -t flask-devops-app .
docker run -p 5000:5000 flask-devops-app
````

## ☸️ Kubernetes (via Minikube)

Start minikube:

```bash
minikube start
kubectl apply -f k8s/
minikube service flask-service
```

## ⚙️ GitHub Actions

I/CD workflow triggers on every push to the `main` branch.

It performs:

- 🐳 Docker build of the Flask app
- 📤 Pushes the image to Docker Hub (`sumit54/flask-devops-assignment`)


## 📝 Author

Sumit Bhatt
[GitHub Repo](https://github.com/sumit-bhatt9/Flask-devops-assignment)
