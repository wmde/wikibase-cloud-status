# status-page

This repository contains the source code for the wikibase.cloud status page.

## Deployment

The status page is deployed to GitHub pages and will be built on each push to the `main` branch.

## Local development

To develop the site locally, use the existing [`docker compose`](https://docs.docker.com/compose/) setup.
Running

```
docker compose up
```

which will start a live-reloading server on <http://localhost:1313>.

## Licenses

All source code in this repository is licensed under the [BSD-3.0 License](./LICENSE).
Page content is licensed as [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
