# Monorepo

## Setup

1. Install Yarn 1.0 or later
2. ...
3. PROFIT!



## Yarn Workspaces

Read the [Yarn Workspaces](https://classic.yarnpkg.com/en/docs/workspaces/)
docs to get familiar with the basic concepts.


### Guidelines

* Every directory in this project should be its own workspace.
* If you need to add a non-workspace directory to version control,
  prefix it with an underscore (e.g. `_save/`) to denote that it is
  NOT a workspace.
* README.md files reserved for information required for development 
  within the monorepo.  These are ignored by 11ty and will not show
  up in the generated documentation.


## Ecosystem

* **Core**
  * platform-independent source
    * data (e.g., design tokens, etc.)
    * graphics (e.g., logos, icons, etc.)
  * ships platform-specific tokens
    * mobile (iOS, Android, etc.)
    * web
    * desktop
    * other...
* **Platform**
  * consumes platform-specific tokens
  * source output is to be extended by platform-specific libraries/toolkits
  * ships platform-specific assets
    * web: HTML, CSS, JavaScript, SVG/PNG/JPG, etc.
    * desktop: EXE/binaries, DLL, ICO, SVG/PNG/JPG, FIG/SKETCH/AI, etc.
    * mobile: JSON, XML, SVG, etc.
* **Library**
  * consumes platform-specific assets
  * source output is to be consumed by application source code
  * ships library-specific assets (e.g., React/Ember/Vue components, etc.)
* **Application**
  * consumes library-specific assets
  * ships a product through various distribution channels
    * web apps: web server, turn-key web service, CDN, etc.
    * mobile apps: app store, file server, etc.
    * desktop apps: app store, file server, etc.


## NOTES

* DO NOT `yarn workspace ... publish` without a clean working directory!
  * yarn will commit all changes if you bump the workspace version via the CLI prompts

