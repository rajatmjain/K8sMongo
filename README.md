# K8sMongo

K8sMongo is a repository that simplifies the deployment and management of MongoDB in a Kubernetes environment. It provides a streamlined approach for running MongoDB as a containerized application, leveraging the power and flexibility of Kubernetes orchestration.

## Features

- Easy Deployment: Deploy MongoDB in a Kubernetes cluster using the provided deployment files.
- Secrets Integration: Securely manage sensitive information, such as usernames and passwords, with Kubernetes secrets.
- Configuration Flexibility: Fine-tune MongoDB's configuration using Kubernetes ConfigMaps.
- External Service Access: Expose the MongoDB service externally using a LoadBalancer service type.

## Getting Started

To get started with K8sMongo, follow these steps:

1. Clone this repository: `git clone https://github.com/rajatmjain/K8sMongo.git`
2. Customize the MongoDB deployment by modifying the deployment file and adjusting the configuration as needed.
3. Configure the necessary secrets for MongoDB authentication.
4. If required, update the MongoDB configuration using the provided ConfigMap file.
5. Deploy MongoDB in your Kubernetes cluster using the deployment file: `kubectl apply -f mongodb-deployment.yaml`
6. (Optional) Expose the MongoDB service externally: `kubectl apply -f mongodb-service.yaml`


## Contributing

Contributions to K8sMongo are always welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request.


## Acknowledgments

K8sMongo was created and is maintained by Rajat Jain. I would like to express my gratitude to the open-source community for their valuable contributions.

