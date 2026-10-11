# DevOps Lab

A hands-on DevOps engineering project focused on building, deploying, securing, and monitoring a containerized application using modern DevOps practices.

## Project Goals

- Develop and test a Python API.
- Manage source code using Git and GitHub.
- Containerize the application with Docker.
- Build automated CI/CD pipelines with GitHub Actions.
- Deploy and manage workloads on Kubernetes.
- Implement infrastructure automation and monitoring.
- Apply security scanning and DevSecOps practices.

## Current Technology Stack

- **Application:** Python, FastAPI
- **Version Control:** Git, GitHub
- **Development Environment:** Ubuntu Server
- **API Server:** Uvicorn

## Application Endpoints

| Endpoint | Description |
|---|---|
| `/` | Returns a welcome message |
| `/health` | Returns the application health status |
| `/docs` | Interactive API documentation |

## Run Locally

Clone the repository:

```bash
git clone git@github.com:yawzup1/devops-lab.git
cd devops-lab
```

Create and activate a Python virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start the application:

```bash
uvicorn app.main:app --host 0.0.0.0 --port 8000
```

Test the API:

```bash
curl http://localhost:8000/
curl http://localhost:8000/health
```

Interactive API documentation is available at `http://localhost:8000/docs`.

## Planned Improvements

- [ ] Add automated application tests with pytest.
- [ ] Create a Dockerfile and Docker Compose configuration.
- [ ] Build CI pipelines using GitHub Actions.
- [ ] Publish container images to GitHub Container Registry.
- [ ] Deploy the application to Kubernetes.
- [ ] Introduce Helm, Terraform, and Ansible.
- [ ] Add monitoring, logging, and security scanning.

## Learning Approach

This repository documents a practical, step-by-step DevOps learning journey. Each improvement will be version-controlled and introduced through focused commits.

---

*This project is actively being developed as part of a hands-on DevOps engineering portfolio.*
