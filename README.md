# Markdown Viewer

A tiny GitHub Pages app that reads base64-encoded markdown from the URL, decodes it, and renders it in the browser.

## Usage

Preferred GitHub Pages form:

```text
https://<user>.github.io/md-viewer/#<base64-markdown>
```

Use the hash form for large markdown. URL fragments are not sent to GitHub's server, so they avoid GitHub Pages `URI Too Long` errors.

Also supported for short markdown only:

```text
https://<user>.github.io/md-viewer/?md=<base64-markdown>
https://<user>.github.io/md-viewer/<base64-markdown>
```

URL-safe base64 is supported (`-`/`_` instead of `+`/`/`).

## Deploy

Push to `main`, then in GitHub set:

- Settings → Pages → Source: **GitHub Actions**

The included workflow deploys the static site automatically.
