# Homepage for Seroanalytics.org

## Requirements
* Jekyll: https://jekyllrb.com/docs/installation/

## Adding/modifying tools
Tools are configured in 3 yaml files:
* `_data/model.yml`
* `_data/simulate.yml`
* `_data/visualise.yml`

You must provide a name, description and gh repo for each tool, plus an optional logo, 
docs link, and link to a web app

e.g. a complete entry looks like:
```yaml
- name: "seroviz"
  description: "SeroViz is an online tool for visualising surveillance and exposure data. Scale and disaggregate, fit splines, and download plots."
  docs: "/seroviz"
  logo: "seroviz.png"
  gh_repo: seroviz
  web: "https://seroviz.seroanalytics.org"
```

The html template for displaying a tool is in `_includes/tool.html`.

There is just one page, `index.md`, the appearance of which is controlled by the `_layouts/default.html` template.

## Serving locally
Run `jekyll serve` to build the site locally. 
