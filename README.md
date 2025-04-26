# Quant Dev Env 🧠📈

A lightweight, containerized development environment for quantitative research, featuring JupyterLab and a fully integrated KDB+/q database server.

## 🚀 Features
- 📦 Isolated Dockerized environment for reproducibility
- 📊 JupyterLab interface with preinstalled Python libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`)
- 🧠 Integrated KDB+/q server for time-series data storage and real-time analytics
- 🔒 Safe local sandbox for developing quant trading strategies and pipelines
- 🌐 Easily extensible to cloud services (AWS EC2, S3)

## 📁 Project Structure
```bash
quant-dev-env/
├── docker-compose.yml         # Orchestrates services
├── services/
│   ├── jupyter/
│   │   └── Dockerfile          # Sets up Python/Jupyter environment
│   └── kdb/
│       ├── Dockerfile          # Sets up custom KDB+ environment
│       ├── q.k                 # KDB+ startup script (user must supply)
│       ├── k4.lic              # KDB+ license file (user must supply)
│       └── l64/                # KDB+ executable directory (user must supply)
├── notebooks/
│   └── intro.ipynb             # Jupyter notebooks live here
├── README.md                   # This file
└── .gitignore                  # Keeps sensitive/binary files out of version control
```
## 📓 Included Notebooks
intro.ipynb: Walkthrough of core tools (pandas, numpy, etc.)

## 🛠️ Usage
1. Obtain KDB+ Personal Edition:
    - Download the Linux version from KX Downloads.
    - Place the following inside services/kdb/:
        - q.k
        - k4.lic
        - l64/ directory (containing the q binary)

    ⚠️ Important: Due to licensing restrictions, KDB+ files are not included in this repository.

2. Clone the repository:
```bash
git clone https://github.com/TreyAllan/quant-dev-env.git
cd quant-dev-env
```

3. Build and run the environment:
```bash
docker-compose up --build
```

4. Access your services:
    - JupyterLab: http://localhost:8888
    - KDB+: Accessible internally on port 6000

5. Stopping services:
```bash
docker-compose down
```

## 🌱 Future Enhancements
- Real-time tick data ingestion
- AWS EC2 deployment setup
- Front-end dashboard using AWS Amplify
- Automated trading simulations with historical data

## 👤 Author
Trey Allan Jean-Baptiste
- github.com/TreyAllan
