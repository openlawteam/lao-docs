# LAO Docs

![Linters status](https://github.com/openlawteam/lao-docs/workflows/Format/badge.svg)
[![Netlify Status](https://api.netlify.com/api/v1/badges/8dd1a66b-ca28-43ee-978d-0a95e7fefff7/deploy-status)](https://app.netlify.com/sites/thelao-docs/deploys)

## Editing

### File structure

All docs are found in the [`/docs`](/docs) directory.

### Format

Uses standard [CommonMark] markdown spec formatting, with default VuePress
[Markdown Extensions].

[commonmark]: https://spec.commonmark.org/current/
[markdown extensions]: https://vuepress.vuejs.org/guide/markdown.html

### Local Development

If you wish to be able to see changes reflected live, you can run a local dev
server. Requires a NodeJS environment on your machine.

> Run `npm ci` to quickly install all necessary dependencies. You can then run
> `npm run docs:dev` to launch a local live-reload instance of the docs. Changes
> will be reflected as soon as you save the source file.

You can also run `npm run docs:build` if you ever want to manually build the
static output. This is normally handled on the CI server automatically. For
consistent code formatting we use [Prettier], if you wish you can format all
files prior to a commit via `npm run format`.

[prettier]: https://prettier.io

### vscode Workspace Settings

VSCode workspace settings are included in this repository, when opening for the
first time you should be prompted to install some recommended extensions. Once
installed, you should automatically get:

- Syntax highlighting and snippets for "stylus" files
- Automatic code formatting via `prettier` on file save

### Image optimization

Please make sure that if you add new image files, it's done via a Pull Request.
Images will then be automatically optimized for filesize in CI! :-)

## Deployment

Deployment is handled automatically via Netlify. :tada: Any needed
customizations can be made in the `netlify.toml` file.

## License

The written documentation and source code examples are licensed under the
[Creative Commons Attribution 4.0 International][license] license.

[license]: https://creativecommons.org/licenses/by/4.0/
