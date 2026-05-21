# Security Notes

## Recommendations

- Do not hardcode MongoDB usernames or passwords in source code.
- Store secrets in environment variables or Kubernetes Secrets.
- Do not commit `.env` files to GitHub.
- Restrict Kubernetes access using RBAC.
- Use separate credentials for development and production environments.

## Future Improvements

- Add external secret management
- Add TLS for MongoDB connections
- Add CI security scanning
