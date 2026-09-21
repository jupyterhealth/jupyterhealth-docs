# JupyterHealth Documentation

The landing site for the JupyterHealth documentation and broader ecosystem.
This describes what the project is, and where to find the docs for each piece.

This is a complement to https://jupyterhealth.org, which serves more as a _brochure site_.
This site is more of a definitive project-wide documentation.

## Preview the site locally

Preview locally with [nox](https://nox.thea.codes):

```bash
nox -s docs:live
```

## Shared navbar and footer

This is a MyST site, and provides [shared MyST configuration](https://mystmd.org/guide/configuration#composing-myst-yml) that other documentation sites can use.
Find those in: `docs/_site/site.yml`.

To reuse that configuration in another MyST site, add this to its `myst.yml`:

```yaml
extends:
  - https://raw.githubusercontent.com/jupyterhealth/jupyterhealth-docs/main/docs/_site/site.yml
```

The footer needs the footer plugin, so also add it to the site's `project.plugins`:

```yaml
plugins:
  - https://github.com/jupyter-book/myst-plugins/releases/download/footer-latest/index.mjs
```
