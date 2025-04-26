# Use a lightweight Python base image
FROM python:3.13-slim

# Set working directory
WORKDIR /app

# Install pip packages
RUN pip install --no-cache-dir \
    jupyterlab \
    pandas \
    numpy \
    matplotlib \
    seaborn

# Expose Jupyter port
EXPOSE 8888

# Run Jupyter Lab on container start
CMD ["jupyter", "lab", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]
