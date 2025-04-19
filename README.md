# 🎂 Birthday Reminder App - Kubernetes Deployment on DigitalOcean

This is a lightweight Flask web app deployed using Docker and Kubernetes on DigitalOcean Kubernetes (DOKS). It includes autoscaling and load balancing, and is optimized for cost and performance.

---

## 🔧 Prerequisites

- Docker Desktop (Windows)
- PowerShell
- Git
- [kubectl](https://kubernetes.io/docs/tasks/tools/)
- [doctl](https://docs.digitalocean.com/reference/doctl/)
- A Docker Hub account
- A DigitalOcean account

---

## 🚀 Local Setup & Build

```powershell
git clone https://github.com/jeffingn/birthday-reminder.git
cd birthday-reminder

docker build -t birthday-reminder-app .
docker tag birthday-reminder-app YOUR_DOCKERHUB_USERNAME/birthday-reminder-app:latest
docker push YOUR_DOCKERHUB_USERNAME/birthday-reminder-app:latest
