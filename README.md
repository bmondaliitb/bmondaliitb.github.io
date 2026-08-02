# Buddhadeb Mondal — portfolio

A small, Markdown-first Jekyll site for GitHub Pages. There is no JavaScript framework, CMS, or remote theme.

## Edit content

- Homepage: `index.md`
- Research overview: `research/index.md`
- Individual research notes: `_research/*.md`
- Project overview: `projects/index.md`
- Individual projects: `_projects/*.md`
- CV and talks: `cv/index.md`
- Selected papers: `publications/index.md`

Each research or project file starts with a short YAML block. Edit fields such as `summary`, `period`, `status`, `stack`, and `featured`; write the longer description below it in normal Markdown. New files in either collection become pages automatically.

Set `featured: true` to show an item on the homepage. Lower `order` values appear first.

## Preview locally

```bash
bundle install
bundle exec jekyll serve
```

Open <http://127.0.0.1:4000>. GitHub Pages uses the same Jekyll build.

On Fedora, Bundler may first require the native build tools: `sudo dnf install ruby-devel gcc gcc-c++ make redhat-rpm-config`. This is only for local preview; GitHub Pages performs its own build after publishing.

## Publish

The personal-site repository is `bmondaliitb/bmondaliitb.github.io`. Its Pages site is <https://bmondaliitb.github.io/>. Commit these files to the branch configured as the GitHub Pages source (currently `gh-pages` in the remote repository), then check **Settings → Pages** if the deployment does not start automatically.

Before publishing, review the contact email, the “300+ publications” wording, private-project visibility notes, and any collaboration approval requirements for research material.

## Visual sources

- `assets/images/ttgamma-photon-pt.png`: ATLAS Collaboration / HEPData, JHEP 10 (2024) 191, [dataset DOI](https://doi.org/10.17182/hepdata.146899), CC BY 4.0.
- `assets/images/thought-breaker.png`: screenshot from the local Thought Breaker project.
- `assets/images/tagore-artwork.webp`: artwork asset from the local Tagore Radio project.
- `assets/images/calorimeter-ml.svg`: original explanatory schematic for this website; fully editable SVG.
