# How to Customize

You can expand or rewrite parts of the theme.

_MkDocs offers a [generic, detailed guide to customizing a MkDocs theme](https://www.mkdocs.org/user-guide/customizing-your-theme/){target="_blank"}._

[TOC]

## Stylesheets

Add your own CSS files to override the theme's default styles:

```yaml
extra_css:
    - css/custom.css
```

## JavaScript

Add your own JavaScript files to extend the theme's functionality:

```yaml
extra_javascript:
    - js/custom.js
```

## Templates & Assets

Override templates and assets of [TACC theme](https://github.com/TACC/mkdocs-tacc/tree/main/mkdocs_tacc/tacc_readthedocs) or [ReadTheDocs theme](https://github.com/mkdocs/mkdocs/tree/1.4.2/mkdocs/themes/readthedocs) e.g.

- **`img/logo.svg`**
- `img/favicon.ico`
- `main.html`
- `nav.html`
- `footer.html`
- `searchbox.html`

To override a template:

1. Create a directory called `overrides` in your docs directory.
2. Add your custom templates e.g.

    ```
    docs/
    ├── overrides/
    │   ├── main.html
    │   └── footer.html
    ```

3. Configure overrides via `mkdocs.yml`:

    ```yaml
    theme:
        name: tacc_readthedocs
        custom_dir: overrides
    ```

## More Options

- [MkDocs: User Guide: Customizing Your Theme](https://www.mkdocs.org/user-guide/customizing-your-theme/){target="_blank"}
- [TACC/mkdocs-tacc: Configuration](configure.md)
- [TACC/mkdocs-tacc: Supported Extensions](extensions.md)