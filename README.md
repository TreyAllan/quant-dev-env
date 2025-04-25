# Quantitative Research Prototyping Environment

## Overview:
This project provides a Dockerized environment for quantitative research and analysis using Python. It allows you to quickly spin up a reproducible environment with all the necessary tools for time-series data analysis, backtesting strategies, and more.

## Getting Started:
Follow the steps below to run this project locally.

### Prerequisites:
- Docker
- Docker Compose

### Installation:
1. Clone this repository:
    ```bash
    git clone https://github.com/your-repo/quant-dev-env.git
    cd quant-dev-env
    ```

2. Build the Docker container:
    ```bash
    docker-compose up --build
    ```

3. Open Jupyter Lab in your browser:
    ```bash
    http://127.0.0.1:8888/lab
    ```

4. Start using the notebooks in the `notebooks/` folder.

### Dependencies:
- pandas
- numpy
- matplotlib
- jupyterlab

### License:
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

