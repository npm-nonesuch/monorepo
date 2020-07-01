# Monorepo Documentation

## Thoughts

* Static-Site Generator: [11ty](https://www.11ty.dev/)
    * Can "reach into" each package for documentation.
    * Generate ONE docs site for ALL packages.
        * File Path: `packages/foo/*` -->
        * URL Path: `/foo/*`
    * One NPM script to run to publish ALL documentation to Netlify, Zeit, GitHub pages, etc.

## Questions

1. Would it still be possible to include Storybook-generated content for specific packages?
    * What if `no-web-ember`, `no-web-react`, etc. want to use Storybook for component docs?
        * Maybe need a standard npm script to run (`npm run build:docs`).
        * Maybe output generated content to a standard directory (e.g., `packages/**/dist/docs`).

