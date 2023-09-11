# splashpage-template
An event landing page built on a [Tech Conference Theme](https://themes.3rdwavemedia.com/demo/bs5/devconf/)

For linked splashpage and JupyterBook see https://github.com/uwhackweek/jupyterbook-template

## How to use this template

You can use this template for your own event!

1. Click the "Use this template" button at the top of the repo
1. Select the account where you'd like to use the template.
1. In your new repo, got to Settings --> Pages --> Source = GitHub Actions
1. There are a few files you'll need to edit to customize content for your event:
  * `cookiecutter.yaml`:  customize your landing page content
1. Any commits pushed to the main branch will be published to GitHub Pages!

## Build website locally

First create an environment with necessary python packages
```
cd [repository]
mamba env create
mamba activate splashpage
```

Then run the build script
```
./scripts/build_resources.sh
```

And preview your webpage!
```
open _build/html/index.html 
```

## Details

This template uses simple text YAML files to fill in key website details. [Cookiecutter](https://cookiecutter.readthedocs.io/en/stable/README.html) is then used to populate templated HTML for the final webpage.
