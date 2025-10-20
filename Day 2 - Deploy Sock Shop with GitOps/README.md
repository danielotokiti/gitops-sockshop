# Day 2 – Deploying Sock Shop with Argo CD (GitOps Workflow)

## Tasks Completed:
- Added the **Sock Shop** Kubernetes manifests (Deployments, Services, and Namespace) to the `app/sock-shop/` folder in the repository.
- Installed **Argo CD** in the `argocd` namespace and accessed its UI via port-forwarding.
- Created an Argo CD Application manifest (sockshop-app.yaml) pointing to the GitHub repo path containing the Sock Shop YAML files.
- Synced the application through the Argo CD UI, triggering the automated deployment of all Sock Shop microservices to the sock-shop namespace.
- Verified all Pods and Services were created successfully:
- Observed GitOps behavior — manual changes (e.g., scaling) were reverted automatically as Argo CD reconciles the live cluster state with the declared Git state.

# Screenshots:
- Argo CD Application manifest
- Argo CD login page and UI (after port-forward).
- kubectl get pods -n argocd showing Argo CD components running.
- Argo CD “Sock Shop” application card in the UI.
- Sync process visualization showing multiple Sock Shop microservices being deployed.
- kubectl get pods -n sock-shop output showing all app pods running successfully.
- Sock Shop app running locally
