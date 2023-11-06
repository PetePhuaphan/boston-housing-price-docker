# Boston Housing Price Prediction with Streamlit on Docker

This repository showcases a Python machine learning project aimed at predicting housing prices in the Boston area. While the machine learning model is straightforward, the primary objective of this project is to demonstrate the deployment of a machine learning model into a web application, rather than focusing on the intricacies of machine learning algorithms or advanced feature engineering.

The prediction model, trained on the classic Boston Housing dataset, is serialized using pickle. This simplifies deployment, making it a suitable approach for those new to applying machine learning in practical settings. The model is deployed using Docker, which encapsulates the environment and dependencies, thereby simplifying the distribution and execution of the Streamlit web application.

Through the Streamlit interface, users are empowered to interactively manipulate parameters and acquire real-time housing price predictions. This project exemplifies a streamlined method to bring a machine learning model to life within a web application, making it an ideal reference for educational objectives, swift prototyping, or as groundwork for more complex implementations.

## Prerequisites

Before running the application, ensure Docker is installed on your system. You can download and install Docker from [Docker's official website](https://www.docker.com/products/docker-desktop).

## Running the Application with Docker

Follow these steps to get the application up and running:

### 1. Run the Docker Container

Launch the application by creating a container from the pulled image:

```bash
docker run -p 8501:8501 -d peteptpn/boston-housing-ml-streamlit:0.1
```

### 2. Access the Application
After the container starts, open your web browser and go to the following URL to access the Streamlit application:

```bash
http://localhost:8501
```

## Stopping the Container
When you're finished using the app, you can stop the Docker container with:

```bash
docker stop <container_id>
```

To find the <container_id>, list all running containers with:

```bash
docker ps
```

### Accessing the App Without Docker

If you prefer not to use Docker, the Boston Housing Price Prediction app is also available on the Streamlit sharing platform. You can access it directly at:

[https://boston-housing-price.streamlit.app/](https://boston-housing-price.streamlit.app/)

Please note that if the app hasn't been used for a while, it may be in a hibernation state. In that case, it might take a short moment for the app to wake up and become responsive.

This web version allows you to interact with the application without any installations or local setup.
