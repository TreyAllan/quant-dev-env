# Quant Dev Env 🧠📈

A lightweight, containerized development environment for quant and data-driven projects using JupyterLab, Python, and Docker.

## 🚀 Features

- 📦 Runs in Docker with isolated dependencies
- 📊 JupyterLab interface with preinstalled libraries (`pandas`, `numpy`, `matplotlib`)
- 🔒 Safe local sandbox for experimenting with quant strategies and data pipelines
- 🧪 Easy to extend with additional tools (e.g., KDB+/q, PostgreSQL, etc.)

## 📁 Project Structure

quant-dev-env/
├── docker-compose.yml       # Orchestrates services
├── Dockerfile               # Sets up Python/Jupyter environment
├── notebooks/               # Jupyter notebooks live here
└── README.md                # This file

## 📓 Included Notebooks
intro.ipynb: Walkthrough of core tools (pandas, numpy, etc.)

## 🛠️ Usage
```bash
git clone https://github.com/yourusername/quant-dev-env.git
cd quant-dev-env
docker compose up
```

Visit: http://localhost:8888 and start coding.

## 🌱 Future Plans
Integrate KDB+/q support

Add time-series finance datasets

Enable automatic AWS deployment

## 👤 Author
Trey Allan Jean-Baptiste
github.com/TreyAllan
