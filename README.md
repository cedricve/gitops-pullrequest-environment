# GitOps action for creating/updating/deleting a PR envrionment

This action allows to create a pull request on a remote GitOps repository.

Example usage:

```yaml
steps:
  - name: Create GitOps Pull Request Envrionment
    uses: cedricve/gitops-pullrequest-action@master
    with:
      action: "create"
      github-token: ${{ secrets.TOKEN }}
      gitops-repo: "uug-ai/gitops"
      gitops-pr-environment: "pr244"
      commit-email: "gitops@uug.ai"
      commit-name: "GitOps"
      commit-mesage: "A new pull request environment for Kerberos Hub xxx"
```
