# Skyward

An illustrated aviation guide built with plain HTML, CSS, and JavaScript.

## Features

- Aviation home page with an interactive guide to the four forces of flight
- Six civilian aircraft category pages
- Six military aircraft category pages
- Filterable aircraft collections and responsive navigation
- Locally hosted WebP aircraft imagery (AI-generated category illustrations)

## Run locally

No dependency installation or build step is required. From the repository root:

```sh
python3 -m http.server 8000 --directory dist
```

Open http://localhost:8000 in your browser. Serve `dist` at the web root because page and asset links use root-relative paths.

## Project structure

- `dist/index.html` — home page
- `dist/aircraft.html` — civilian aircraft collection
- `dist/military.html` — military aircraft collection
- `dist/aircraft/` — individual aircraft guides
- `dist/assets/` — CSS, JavaScript, and WebP images
- `.openai/hosting.json` — original Sites hosting configuration

## Deployment

Publish `dist` as the static document root. A server-side application or build command is not needed. This repository does not automatically configure hosting or CI/CD.

## Content and imagery

The guides describe aircraft categories, not specifications for individual models. Military guides link to official reference material. Aircraft images are AI-generated visualizations and are not photographs or technical representations of the reference models.
