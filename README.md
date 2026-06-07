# Markdown Viewer

A tiny GitHub Pages app that reads base64-encoded markdown from the URL, decodes it, and renders it in the browser.

## Usage

Preferred GitHub Pages form:

```text
https://<user>.github.io/md-viewer/?md=<base64-markdown>
```

Also supported:

```text
https://<user>.github.io/md-viewer/#<base64-markdown>
https://<user>.github.io/md-viewer/<base64-markdown>
```

URL-safe base64 is supported (`-`/`_` instead of `+`/`/`).

## Deploy

Push to `main`, then in GitHub set:

- Settings → Pages → Source: **GitHub Actions**

The included workflow deploys the static site automatically.
