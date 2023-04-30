# K8sMongo

K8sMongo is a repository that simplifies the deployment and management of MongoDB and mongo-express in a Kubernetes environment. It provides a streamlined approach for running MongoDB and mongo-express as containerized applications, leveraging the power and flexibility of Kubernetes orchestration.

## Features

- Easy Deployment: Deploy MongoDB and mongo-express in a Kubernetes cluster using the provided deployment files.
- Secrets Integration: Securely manage sensitive information, such as usernames and passwords, with Kubernetes secrets.
- Configuration Flexibility: Fine-tune MongoDB and mongo-express configurations using Kubernetes ConfigMaps.
- External Service Access: Expose the MongoDB and mongo-express services externally using LoadBalancer service types.

## Getting Started

To get started with K8sMongo, follow these steps:

1. Clone this repository: `git clone https://github.com/rajatmjain/K8sMongo.git`
2. Customize the MongoDB deployment by modifying the deployment file (`mongodb-deployment.yaml`) and adjusting the configuration as needed.
3. Configure the necessary secrets for MongoDB authentication in the `mongodb-secret.yaml` file.
4. If required, update the MongoDB configuration using the provided ConfigMap file (`mongodb-configmap.yaml`).
5. Deploy MongoDB in your Kubernetes cluster using the deployment file: `kubectl apply -f mongodb-deployment.yaml`
6. (Optional) Expose the MongoDB service externally: `kubectl apply -f mongodb-service.yaml`
7. Customize the mongo-express deployment by modifying the deployment file (`mongoexpress-deployment.yaml`) and adjusting the configuration as needed.
8. Configure the necessary secrets for mongo-express authentication in the `mongodb-secret.yaml` file (if not already configured).
9. If required, update the MongoDB server URL configuration for mongo-express using the provided ConfigMap file (`mongodb-configmap.yaml`).
10. Deploy mongo-express in your Kubernetes cluster using the deployment file: `kubectl apply -f mongoexpress-deployment.yaml`
11. (Optional) Expose the mongo-express service externally: `kubectl apply -f mongoexpress-service.yaml`
12. (Optional) Expose the mongo-express ingress externally: `kubectl apply -f mongoexpress-ingress.yaml`
13. (Optional) Create a mapping between the host and IP through `sudo vim /etc/hosts`, example: `192.168.64.5  mongoexpressk8s.com`
14. (Optional) Access mongoexpress-service by going to `http://mongoexpressk8s.com` in the browser.

## Contributing

Contributions to K8sMongo are always welcome! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

K8sMongo was created and is maintained by Rajat Jain. I would like to express my gratitude to the open-source community for their valuable contributions.
