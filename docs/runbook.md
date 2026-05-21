# Deployment Runbook

## Local Startup

1. Deploy MongoDB resources to Kubernetes
2. Seed the database
3. Port-forward MongoDB locally
4. Configure environment variables
5. Start the Gradio application

## Validation

- Verify Kubernetes pods are running
- Verify MongoDB collections exist
- Verify Gradio UI loads on port 7860
- Ask sample questions to validate responses

## Troubleshooting

### MongoDB unavailable

Check:

```bash
kubectl get pods -n fifa2026
```

### Port-forward issues

Restart:

```bash
kubectl port-forward -n fifa2026 svc/mongodb-service 27017:27017
```
