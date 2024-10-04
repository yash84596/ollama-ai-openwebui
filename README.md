# ollama-ai-openwebui
**Private Ollama AI Deployment**  Deploy over 20 AI models locally or in the cloud using Docker containers and a user-friendly interface. Keep your data secure and access AI capabilities without relying on third-party services. Ideal for businesses and individuals seeking control over their AI deployments.

**Features**

- Deploy over **20 AI models** from Ollama.
- Integrated **OpenWebUI** for easy and interactive access to models.
- Supports **local offline and cloud deployment** (AWS EC2).
- Ensures **privacy** by keeping all data within your infrastructure.
- Easy to set up using **Docker containers.**

**System Requirements**

List the minimum system or hardware requirements for running the project, both locally and on the cloud.

**Hardware Requirements:**
- 8-16 GB RAM
- 4-core CPU

**Software Requirements:**
- Docker (version 20.x or above)
- Docker Compose (version 1.29 or above)
- AWS EC2 (optional for cloud deployment)

**Installation Guide**
1. Clone the repository:
   ```bash
   git clone https://github.com/abhay-dandge/ollama-ai-openwebui.git
   cd ollama-ai-openwebui

2.Build and start the Docker containers:

   ```bash
   docker-compose up --build
```
3. Access the OpenWebUI at http://localhost:8080 to interact with the AI models.

**AWS EC2 Deployment**

1.Launch an EC2 instance with the following specs:

    8-16 GB RAM
    4-core CPU
    Ubuntu 20.04 AMI

2. Install Docker and Docker Compose on the EC2 instance:
   ```bash
   sudo apt update
   sudo apt install docker.io docker-compose
   ```
3. Clone the repository and start the containers:
   ```bash
   git clone https://github.com/abhay-dandge/ollama-ai-openwebui.git
   cd ollama-ai-openwebui
   docker-compose up --build
   ```bash
4. Access the OpenWebUI at http://<your-ec2-public-ip>:8080.

   - Once the containers are running, access the UI via http://localhost:8080 or http://<your-ec2-public-ip>:8080 on the cloud.
   - Choose from the list of AI models available in the UI.
   - Interact with the models by inputting text queries or uploading relevant data.
   - For offline use, ensure that your models are pre-downloaded and the containers are running in an isolated environment.

**Data Privacy & Security**

This project ensures complete privacy of your data by allowing you to run AI models on your local infrastructure or in a private cloud. No data is sent to external servers, and all interactions with the models remain within your control. This makes the project suitable for sensitive applications in healthcare, finance, legal, and other industries where data privacy is a priority.

For enhanced security, we recommend using SSL certificates for encrypted communications and setting up access controls for user authentication.

Contributing

We welcome contributions from the community! To contribute:

   1) Fork the repository.
    2) Create a new branch for your feature or fix.
     3) Make your changes and test thoroughly.
      4) Submit a pull request with a detailed description of your changes.

Contact

Created by Abhay Dandge. Feel free to reach out via LinkedIn or GitHub.
