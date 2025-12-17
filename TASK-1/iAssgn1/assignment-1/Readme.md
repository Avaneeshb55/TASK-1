
# Assignment 1: Nginx Docker Server

## Approach Explanation
For this task, I created a containerized web environment using Nginx. I prepared a custom `index.html` file and configured a `Dockerfile` to copy this file into the Nginx default directory.

## Folder Content
This folder follows the required structure and contains:
* **index.html**: Contains my name, a heading, and a brief description.
* **Dockerfile**: Instructions to build the server image using Nginx.
* **README.md**: This file, providing instructions and approach details.

## Commands Used

### 1. Build the Image
To build the image with the name avaneeshb-site:
```bash
docker build -t avaneesh-site .
```

### 2.Run the container
To run a detached container named my-assignment-container , exposing port 7070 on your machine system with service provided at port 80 of the container:
```bash
docker run -d -p 7070:80 --name my-assignment-container avaneesh-site
```

### 3.Testing
Open in browser : localhost:7070<br>
Or test via CLI
```bash
curl http://localhost:7070
```

### 4.Stop the container
```bash
docker stop my-assignment-container
```

### 5.Destroy the container
```bash
docker rm my-assignment-container
```
### 6.Screenshot of curl results
![Curl Output Screenshot](curl-output.png)

