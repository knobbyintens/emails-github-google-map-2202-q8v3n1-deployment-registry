# Deployment Registry — Entry Guide

Each monitoring site is one Markdown file in `_registry/`, named
`<deployed-date>-<site-slug>.md` (for example `2024-03-12-harbor-elementary.md`).

The file starts with a YAML front matter block:

| field       | value                                                        |
|-------------|--------------------------------------------------------------|
| `title`     | display name of the site                                     |
| `site_type` | one of `library`, `school`, `transit`, `park`, `market`, `clinic` |
| `address`   | street address of the site                                   |
| `latitude`  | decimal degrees, from the site address                       |
| `longitude` | decimal degrees, from the site address                       |
| `deployed`  | go-live date, `YYYY-MM-DD`                                   |
| `status`    | `planned`, `active` or `retired`                             |
| `dataseturl`| link to the site's published dataset repository              |

`dataseturl` is optional: it exists only for sites whose dataset repository is
already published under our own GitHub account. Never point it at a mirror,
fork, or third-party copy, and never point it at a repository whose data is not
yet available to the public.

The body of the file is one or two sentences describing the site.
