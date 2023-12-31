# Part One: Setting up your Kubernetes cluster

## Objectives
- Choose your platform: Select your preferred platform mentioned and follow their setup instructions I will be using Docker Desktop however once you have your dev cluster up and running all the kubernetes commands will be the same regardless of what platform you choose.
- Verify cluster access: Once setup, test access to your cluster using kubectl get nodes.


## steps to set up a Kubernetes cluster using Docker Desktop:

1 Installation and Requirements:

Install Docker Desktop: Download and install the latest version of Docker Desktop for your operating system from https://www.docker.com/products/docker-desktop.
System Requirements: Ensure your system meets the minimum requirements for Docker Desktop, which include:
Virtualization enabled in BIOS (for Windows and macOS)
4GB of RAM (8GB recommended)
2 CPUs (4 CPUs recommended)
Enable Kubernetes:
Open Docker Desktop preferences and go to the "Kubernetes" tab.
Check the box to "Enable Kubernetes".
Click "Apply & Restart" to enable the Kubernetes cluster.
2. Verification and Access:

Verify Cluster Status:
Open a terminal or command prompt.
Run kubectl get nodes to check if the Kubernetes cluster is running. You should see a single node in the "Ready" state.
Accessing the Cluster:
Docker Desktop automatically configures kubectl for you, so you can directly use kubectl commands to interact with the cluster.
3. Additional Considerations:

Resources: The Kubernetes cluster within Docker Desktop is intended for local development and testing. It has limited resources compared to cloud-based clusters.
Single-Node Cluster: The cluster consists of a single node, which means you won't be able to test features like high availability or multi-node deployments.
Persistence: Persistent volumes created within the cluster are not persistent across Docker Desktop restarts.
4. Working with the Cluster:

Using kubectl: You can now use kubectl commands to deploy applications, manage resources, and explore Kubernetes features within your local cluster.
Accessing Services: To access services exposed within the cluster from your host machine, you'll need to use the Docker Desktop IP address (usually 127.0.0.1) and the port mapped to the service.

[Getting started YT video]()
