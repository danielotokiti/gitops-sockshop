# **Day 1 – Cluster + ArgoCD Setup**

**Tasks Completed:**
- Created a local multi-node Kubernetes cluster using **Kind** with a custom yaml config file.
- Installed ArgoCD into its own namespace using the official manifests.
- Verified ArgoCD components and services (`argocd-server`, `argocd-repo-server`, `argocd-dex-server`).
- Accessed the ArgoCD UI via port-forwarding (`kubectl port-forward svc/argocd-server -n argocd 8080:443`).
- Retrieved the initial `admin` password from the ArgoCD secret and logged into the UI.

---

Screenshots:
- Cluster creation.
- Output of `kubectl get svc -n argocd` confirming ArgoCD services.
- ArgoCD UI login page accessed via `http://localhost:8080`.

---
