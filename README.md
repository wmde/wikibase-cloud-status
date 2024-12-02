# status-page

This repository contains the source code for the wikibase.cloud status page.

## Adding an incident
In the event of an incident, in addition to reporting it in the incidents mattermost channel you should add and incident here.
This is done by adding a markdown file to [the issues folder](/content/issues). You can follow the example of other incidents
to complete the template.
Unlike our normal code repositories it is acceptable to self-merge PRs in this repo.

## Deployment

The status page is deployed to GitHub pages and will be built on each push to the `main` branch.

### Deploying a preview for review
You can use a fork of this repository to deploy any branch as a preview for review via GitHub Pages.

1. Fork this repository: https://github.com/wmde/wikibase-cloud-status/fork
    - De-select `Copy the main branch only` (otherwise you have to sync your branch after forking)
3. Enable GitHub Pages
    - `Settings` -> `Pages` and select `GitHub Actions` as the source
4. Adjust allowed branches for Pages
    - `Settings` -> `Environments` -> `github-pages` and edit the allowed branches from `main` to `*`
5. Run workflow `Deploy Hugo site to Pages`
    - `Actions` -> agree to enable them -> workflow `Deploy Hugo site to Pages` -> `Run workflow` with the branch you want

The setup is only needed once, you can keep the fork and in case you need to do use this again you just need to sync the branch of your choice and repeat step 5. 

## Local development

__Important__: The `cstate` theme is distributed as a git submodule contained in this repository, and is not pulled by default.
To obtain the theme, you can either use `--recursive` when cloning:

```console
git clone --recursive git@github.com:wbstack/status-page.git
```

or init submodules from within the repository root

```console
git submodule update --init
```

To develop the site locally, use the existing [`docker compose`](https://docs.docker.com/compose/) setup.
Running

```console
docker compose up
```

which will start a live-reloading server on <http://localhost:1313>.

## Licenses

All source code in this repository is licensed under the [BSD-3.0 License](./LICENSE).
Page content is licensed as [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
