# Guild of Educators Website 

This website is a work in progress, it is not yet live.

## Local development 

We are using [Zensical](https://zensical.org/)

To run locally:

```bash
# install dependencies
uv sync

# serve on http://localhost:8000
uv run zensical serve
```
## Adding a resource

Resources live in `docs/resources/`, one Markdown file per resource.

1. Copy an existing resource page (e.g. `docs/resources/scratch-for-educators.md`) and fill it in.
2. Add tags in the frontmatter. A resource can have as many tags as make sense.
3. Add the page to the `Resources` section of `nav` in `zensical.toml`.

The resources index page (`docs/resources/index.md`) lists every tagged page, grouped by tag, automatically.

Try to reuse existing tags so things group together. Tags generally answer one of these questions:

- **What is it about?** e.g. `Pedagogy`, `Python`, `Scratch`, `Assessment`
- **What format is it?** e.g. `Book`, `Tutorial`, `Course`, `Website`, `Video`
- **What does it cost?** e.g. `Free`, `Paid`
