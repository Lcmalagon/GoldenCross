# Predictive Stock Analysis: Unveiling the Power of Golden & Death Crosses

This project is a data-driven approach to analyze whether golden crosses and death crosses are reliable indicators of stock price movement. The analysis is conducted in a Jupyter Notebook running in a Google Cloud VM instance. I found a significant correlation in the 50 Day Moving Average (DMA) and 200 DMA, demonstrating that golden crosses can predict stock price increases over a longer period, and similarly, death crosses can predict a downturn.

![Alternative text for image]([URL of the image](https://s3.cointelegraph.com/uploads/2022-12/f336e087-0733-4773-a38b-6d21aa4bd182.png))


## Getting Started

These instructions will help you get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Access to Google Cloud Platform (GCP) is needed, specifically the ability to create VM instances and Storage Buckets.

### Setting Up the Environment

#### Creating a VM Instance

To create a new VM instance, follow these steps:

```bash
# Select a region and zone for your VM instance.
# Choose a machine type for your VM instance.
# Specify the amount of memory and storage for your VM instance.
# Choose an operating system for your VM instance.
# Create a firewall rule to allow traffic to your VM instance.
```
Region and zone: These refer to the geographic location where your VM instance will be hosted. For instance, you could choose the region "us-central1" and the zone "us-central1-a".

Machine type: This is the size and type of the VM instance. For example, "n1-standard-1" is a 1 vCPU, 3.75 GB memory machine.

Memory and storage: Specify the amount of memory and storage for your VM instance. For example, you might specify 8 GB of memory and 100 GB of storage.

Operating system: Choose an operating system for your VM instance, such as "Ubuntu 18.04 LTS".

Firewall rule: Create a firewall rule to allow traffic to your VM instance. For instance, a firewall rule might allow traffic on port 80 (HTTP) and port 443 (HTTPS).

After creating the VM instance, it will take a few minutes to boot up. Once booted up, you can connect to it using SSH.

Creating a Bucket and Docker Image
To create a bucket and a Docker image, follow these steps:

```bash
# Create a bucket in the Cloud Storage console.
# Create a Dockerfile in the bucket.
# Build the Docker image from the Dockerfile.
```

Bucket: This is a storage location for your data. Create a bucket in the Cloud Storage console.

Dockerfile: This is a text file that describes how to build a Docker image. You can create a Dockerfile in the bucket.

Build the Docker image: You can build the Docker image from the Dockerfile using the following command: 

```bash
docker build -t <image_name> .
```

After creating the Docker image, you can push it to the Docker Hub using the following command: 
```bash
docker push <image_name>
```
Launching a Jupyter Notebook
To launch a Jupyter Notebook from the Docker image, follow these steps:

```bash
# Create a new instance of the Docker image.
# Open a web browser and navigate to the URL for the Jupyter Notebook.
```

Create a new instance of the Docker image: You can do this using the following command: 
```bash
docker run -it -p 8888:8888 <image_name>
```
Open a web browser and navigate to the URL for the Jupyter Notebook: After creating a new instance of the Docker image, open a web browser and navigate to `http://localhost:
