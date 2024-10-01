# Dockerfile
FROM jupyter/base-notebook:python-3.10

# Switch to root user to install packages
USER root

# Update package list and install additional packages
RUN apt-get update && apt-get install -y \
    python3-opengl \
    ffmpeg \
    xvfb \
    && rm -rf /var/lib/apt/lists/*  # Clean up

# Switch back to jovyan user (default user in the base notebook image)
USER jovyan

# Set the working directory
WORKDIR /home/jovyan/work

# Expose port (if needed)
EXPOSE 8888

# Start Jupyter Notebook
CMD ["start-notebook.sh", "--NotebookApp.token=''", "--NotebookApp.password=''", "--notebook-dir=/home/jovyan/work"]
