# Checkout Private Repo

This action checks-out your private repository under `$GITHUB_WORKSPACE`, so your workflow can access it.
You can provide an alternative name of the path to clone it to.

It requires a personal access token with the appropriate permissions to access the private repository.

```yml
  - uses: camyon/checkout-private-repo@v1.0.2
    with:
      repo-url: https://github.com/fortelabsinc/gbu-functional-tests
      ref: develop
      path: tests
      token: ${{ env.GITHUB_SECRET_TOKEN }}
```
    
