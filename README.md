# argocd-copilot

Follow doc from https://argocd-autopilot.readthedocs.io/en/stable/Getting-Started/:

```bash
kind create cluster
export GIT_TOKEN=$(gh auth token)
export GIT_REPO=https://github.com/rbapst-tamedia/argocd-copilot
```

to get password:

```
kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d
```
