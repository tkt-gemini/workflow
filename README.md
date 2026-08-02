<div align="center">

# Dual-Machine

[![WSL](https://img.shields.io/badge/WSL2-Ubuntu--26.04-498AF2?style=for-the-badge)](https://ubuntu.com/wsl)
[![Server](https://img.shields.io/badge/Server-Ubuntu--26.04-D43170?style=for-the-badge)](https://ubuntu.com/server)
[![Version](https://img.shields.io/badge/VERSION-0.1.0-A19654?style=for-the-badge)](https://github.com/tkt-gemini/workflow)
[![License](https://img.shields.io/badge/LICENSE-MIT-6B7F4E?style=for-the-badge)](./LICENSE)

**Workflow for Embodied AI**

</div>

---

## Prerequisites

| Machine | Requirement | Value |
| --- | --- | --- |
| **HP ZBook G11** | OS | Windows 11 · [WSL2](https://github.com/tkt-gemini/wsl) workflow |
| | CPU | Intel Core Ultra 7 165H (22 cores) |
| | RAM | 32 GB |
| | GPU | NVIDIA RTX 1000 Ada (6 GB VRAM) |
| | NPU | Intel AI Boost |
| | Disk | 1 TB SSD |
| **Dell Latitude 7290** | OS | Ubuntu 26.04 LTS (native) |
| | CPU | Intel i5-8350U (4 cores / 8 threads) |
| | RAM | 8 GB |
| | GPU | None (Intel UHD 620) |
| | Disk | 256 GB SSD |

```
┌──────────────────────────────────────┐
│ HP ZBook G11 (Primary Workstation)   │
│ Windows Host + WSL2                  │
│ NVIDIA Driver (CUDA passthrough)     │
└──────────────────┬───────────────────┘
                   │ Tailscale
┌──────────────────▼───────────────────┐
│ Dell Latitude 7290 (Server/CI)       │
│ Ubuntu 26.04 LTS (native)            │
│ Docker · Prometheus · Grafana        │
└──────────────────────────────────────┘
```
