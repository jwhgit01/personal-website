# Personal Website

This is the source repository for Jeremy W. Hopwood's personal website. It is a
Jekyll site that uses the [Beautiful Jekyll](https://beautifuljekyll.com/) remote
theme and [Jekyll Scholar](https://github.com/inukshuk/jekyll-scholar) for the
publications page.

The repository is public so that others can see how the site is put together and
reproduce a similar site from their own repository. It is not intended to be a
fully generic starter template, so expect to replace personal content, site
settings, bibliography entries, images, and navigation with your own.

## How this site is organized

- `_config.yml` contains the site title, author, navigation links, colors,
  logo/avatar settings, URL, plugins, and Jekyll Scholar configuration.
- Markdown files at the repository root provide the main pages, including
  `index.md`, `about.md`, `publications.md`, `teaching.md`, and the research
  pages.
- `_bibliography/references.bib` contains publication data used by
  Jekyll Scholar.
- `_layouts/bib.html` controls the bibliography entry layout.
- `assets/` contains images, CSS, and other static files used by the site.
- `Gemfile` and `Gemfile.lock` define the Ruby/Jekyll dependencies used to build
  the site.

## Reproduce a similar site

1. Create your own repository from this codebase by forking it or copying the
   files into a new repository.
2. Update `_config.yml` with your own title, author, email, description, URL,
   GitHub username, navigation links, colors, and logo/avatar settings.
3. Replace the Markdown page content with your own text and add or remove pages
   to match your navigation.
4. Replace `_bibliography/references.bib` and related bibliography files with
   your own publication data, or remove the publications page and
   `jekyll-scholar` configuration if you do not need bibliography support.
5. Replace images and other static assets under `assets/`, then update any
   references to those files in the Markdown pages or `_config.yml`.
6. Keep `Gemfile.lock` committed so local and hosted builds use the same resolved
   dependency versions.

## Publication bibliography, PDFs, and thumbnails

The publications page is generated from `_bibliography/references.bib` using
Jekyll Scholar and the custom bibliography layout in `_layouts/bib.html`. When
adding or editing publications, check the following repository-specific details:

- Each BibTeX entry key should be stable and unique. The key is used by the
  bibliography layout to find that publication's thumbnail.
- If a BibTeX entry has a custom `file` field, its value should be only the PDF
  filename, for example `file = {myPaper2026.pdf}`. The matching PDF must exist
  at `assets/papers/myPaper2026.pdf`.
- Do not include `assets/papers/` in the `file` field; the layout already adds
  that path when it builds the download link.
- Each publication thumbnail should be a PNG named after the BibTeX key and
  stored in `assets/img/`. For an entry with key `myPaper2026`, use
  `assets/img/myPaper2026.png`.
- Publication thumbnails are displayed at 200 px wide on larger screens and are
  hidden on narrow screens by `assets/css/publications.css`. Use images that are
  clear at that display size; exporting around 400 px wide is a good target for
  high-density displays, while keeping the file size modest for fast page loads.
- Before publishing, verify that every `file` value has a matching PDF and every
  publication you want illustrated has a matching thumbnail.

## Run locally

This site uses Jekyll, Ruby, and Bundler. Setup details vary by operating system,
Ruby version, and Jekyll version, so use the current official documentation for
installation and troubleshooting:

- [Jekyll installation docs](https://jekyllrb.com/docs/installation/)
- [Jekyll quickstart](https://jekyllrb.com/docs/)
- [Bundler documentation](https://bundler.io/docs.html)

After Ruby and Bundler are available, the usual workflow is:

```sh
bundle install
bundle exec jekyll serve
```

Then open the local URL printed by Jekyll. Restart the Jekyll server after
changing `_config.yml` so the configuration is reloaded.

## Build for production

The standard production build command for this repository is:

```sh
bundle exec jekyll build
```

The generated static site is written to `_site/` by default.

## Deploy with Cloudflare Pages and GitHub

This site can be hosted on Cloudflare Pages by connecting Cloudflare to the
GitHub repository. Cloudflare's Pages product appears in the Cloudflare dashboard
under **Workers & Pages**, but a static Jekyll site should be deployed as a
Pages project.

Use Cloudflare's current documentation for the detailed setup flow:

- [Cloudflare Pages: deploy a Jekyll site](https://developers.cloudflare.com/pages/framework-guides/deploy-a-jekyll-site/)
- [Cloudflare Pages Git integration](https://developers.cloudflare.com/pages/configuration/git-integration/)
- [Cloudflare Pages GitHub integration](https://developers.cloudflare.com/pages/configuration/git-integration/github-integration/)
- [Cloudflare Pages custom domains](https://developers.cloudflare.com/pages/configuration/custom-domains/)

For this repository, the important Cloudflare Pages build settings are:

| Setting | Value |
| --- | --- |
| Framework preset | Jekyll |
| Build command | `bundle exec jekyll build` |
| Build output directory | `_site` |

Set the following environment variables for both production and preview builds:

| Variable | Value |
| --- | --- |
| `RUBY_VERSION` | The Ruby version you use locally and want Cloudflare to use for builds |
| `LC_ALL` | `C.UTF-8` |
| `LANG` | `C.UTF-8` |
| `LANGUAGE` | `en_US:en` |

At a high level, the deployment flow is:

1. Push the repository to GitHub.
2. In Cloudflare, create a Pages project from an existing Git repository.
3. Authorize/select the GitHub repository and configure the build settings above.
4. Add the environment variables above in the Cloudflare Pages project settings.
5. Deploy the site and, if desired, attach a custom domain.

After setup, Cloudflare Pages rebuilds and redeploys the site when changes are
pushed to the connected GitHub branch.

## License

See `LICENSE` for the license that applies to this repository.
