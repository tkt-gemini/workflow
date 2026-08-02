```
┌─────────────────────────────────────────────┐
│  HP ZBook G11                               │
├─────────────────────────────────────────────┤
│  Train model (GPU, mixed precision)         │
│  Export model (ONNX, quantize)              │
│  Log run > MLflow/DVC                       │
│  Serve model (FastAPI + CUDA)               │
│  Smoke test after deploy                    │
│  Push code to Git                           │
└─────────────────────────────────────────────┘

┌─────────────────────────────────────────────┐
│  Dell Latitude 7290 - Server                │
├─────────────────────────────────────────────┤
│  Auto-deploy (Git hooks / webhooks)         │
│  Monitor: Prometheus > Grafana              │
│  Backup data (> off-box)                    │
│  CI pipeline orchestration                  │
│  Notification / alerting                    │
└─────────────────────────────────────────────┘
```
