---
icon: lucide/git-pull-request
---

# Contributing Resources

Know a book, course, tutorial, or website that made you a better educator? We'd love to add it. There are two ways to contribute, and you can use whichever you're comfortable with.

- **[Open an issue](#open-an-issue)** if you want to suggest a resource and let someone else write it up. No technical knowledge needed.
- **[Make a pull request](#make-a-pull-request)** if you want to add or improve a resource page yourself.

Both need a free [GitHub](https://github.com/signup) account.

## Open an issue

An issue is a suggestion or request. Someone from the community will pick it up and turn it into a resource page.

1. Go to the [new issue page](https://github.com/Guild-of-Educators/website/issues/new).
2. Give it a title such as "Resource suggestion: The Big Book of Computing Pedagogy".
3. In the description, tell us:
    - **What it is** and a link to it
    - **Who made it** (author or organisation)
    - **Why you recommend it**: what makes it useful for educators?
    - **Who it's good for**, e.g. new teachers, school teachers, bootcamp mentors
    - **Whether it's free or paid**
4. Click **Create**.

You can also open an issue to point out a mistake, a broken link, or a resource that's out of date.

## Make a pull request

A pull request (PR) is a proposed change to the website. Every resource is a single Markdown file in the [`docs/resources/`](https://github.com/Guild-of-Educators/website/tree/main/docs/resources) folder, so adding one means adding one file.

### The easy way: edit on GitHub

You can do the whole thing in your browser.

1. Go to the [`docs/resources/`](https://github.com/Guild-of-Educators/website/tree/main/docs/resources) folder.
2. Click **Add file**, then **Create new file**. GitHub will offer to make a copy of the project (a "fork") for you to work in. Accept it.
3. Name the file after the resource, in lowercase with dashes, ending in `.md`. For example: `the-big-book-of-computing-pedagogy.md`.
4. Paste in the template below and fill it in.
5. Click **Commit changes**, then follow the prompts to **Create pull request**.

### Resource template

```markdown
---
tags:
  - Pedagogy
  - Book
  - Free
---

# Name of the Resource

**By:** Author or organisation
**Link:** <https://example.com>

## What it is

A short description of the resource.

## Why we recommend it

What makes it useful for educators.

## Good for

Who will get the most out of it, e.g. new teachers, school teachers, bootcamp mentors.
```

### Choosing tags

Tags group resources together on the [Resources](index.md) page. A resource can have as many tags as make sense. Try to reuse existing tags so things group nicely. Tags generally answer one of these questions:

- **What is it about?** e.g. `Pedagogy`, `Python`, `Scratch`, `Assessment`
- **What format is it?** e.g. `Book`, `Tutorial`, `Course`, `Website`, `Video`
- **What does it cost?** e.g. `Free`, `Paid`

### Improving an existing resource

Some resource pages still have `TODO` placeholders. If you've used one of these resources, please help fill it in. Open the file in [`docs/resources/`](https://github.com/Guild-of-Educators/website/tree/main/docs/resources), click the pencil icon to edit it, then commit your changes and create a pull request.

### Working locally

If you're comfortable with Git and want to preview your changes before submitting, fork and clone the [repository](https://github.com/Guild-of-Educators/website), then run:

```bash
# install dependencies
uv sync

# serve on http://localhost:8000
uv run zensical serve
```

Add your resource file, check it looks right, then push to your fork and open a pull request.

## What happens next

One of the maintainers will review your issue or pull request. We might ask a question or suggest a few changes. Once it's ready, we'll merge it and your resource will appear on the site.

If you get stuck at any point, ask on our [Discord server](https://discord.gg/8cPdX2bAze). We're happy to help, and nobody minds if it's your first pull request.

All contributions are subject to our [Code of Conduct](../code-of-conduct.md).
