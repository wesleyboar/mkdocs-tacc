# How to Deploy

Deploys rely on [GitHub Pages](https://pages.github.com/) and [MkDocs command `gh-deploy`](https://www.mkdocs.org/user-guide/deploying-your-docs/).

1. Run
    ```shell
    poetry run mkdocs gh-deploy --force --theme tacc_readthedocs
    ```
2. Wait for [GitHub action](https://github.com/TACC/mkdocs-tacc/actions) to complete.
3. Load https://tacc.github.io/mkdocs-tacc/.

# Related

- [How to Publish](./PUBLISHING.md)
