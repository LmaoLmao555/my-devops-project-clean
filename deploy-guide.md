# 🚀 Deployment Guide – ระบบจองห้องประชุม

## 1. Clone repository
```bash
git clone https://github.com/your-user/your-repo.git
cd your-repo
```

## 2. Build Docker image
```bash
docker build -t meeting-room-app .
```

## 3. Deploy to Kubernetes cluster
```bash
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/hpa.yaml
```

## 4. ตรวจสอบสถานะ
```bash
kubectl get pods
kubectl get svc
```

## 5. Optional: เชื่อมกับ Ingress, Alertmanager หรือ Prometheus