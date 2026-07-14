# Argo CD GitOps homework

This private repository is the declarative source of truth for the Argo CD
homework deployment.

Repository layout:

- `bootstrap/` contains the root Argo CD Application;
- `manifests/` contains the AppProject, child Application and SealedSecrets;
- `infrastructure/` contains the reproducible Argo CD Helm values.

The Jenkins child Application deploys the published
`jenkins-homework` Helm chart from:

```text
https://antonzhdanko.github.io/sa2-35-26-jenkins/
```

No plain-text passwords, access tokens or SSH private keys are committed.

