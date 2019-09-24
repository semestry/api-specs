# api-specs

This repository contains API specifications and generated documentation for Eveoh's APIs.

## Publishing

The OpenAPI 3.0 specifications are generated using ReDoc. 
Production API documentation pages are automatically published by Github Pages when changes are pushed to the `master` branch.

## Development

### Viewing documentation locally

Specifications can be served locally using Yarn commands:

`yarn serve:<spec>`

For example:

`yarn serve:echo-webhooks`

Documentation is available at `http://localhost:3000`.

Changes to source files are automatically processed, although your browser should be manually refreshed.

### Linting specifications

Linting is performed using Speccy.

Lint the specs using the following Yarn command:

`yarn lint`

### Adding a API specification

- Add the OpenAPI 3.0 file to `/spec`.
- Create a HTML file in `/docs` serving the specification.
- Add a link to the specification in `/docs/index.html`. 
- Add a `lint:<spec>` script in `package.json`.
- Add a `serve:<spec>` script in `package.json`.
