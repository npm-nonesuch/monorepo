## Content
- Assume
  - platform: `web`
  - framework: `none`

### Pattern Library
- Focus on vanilla HTML+CSS examples.
- JavaScript/behavior docs will be included with the framework-specific components

_format:_
```sh
patterns/{pattern}[/*]
```

_examples:_
```sh
patterns/button
patterns/menu
patterns/table
```


### Guides
_format:_
```sh
guides/{guide}[/*]
```
_examples:_
```sh
guides/accessibility/...
```


## Package Docs
If a package has special docs (i.e., Storybook), slot them in here.

### Paths
_format:_
```sh
packages/{package}
```

_examples:_
```sh
packages/nds-web-angular  # Angular 2+
packages/nds-web-ng       # AngularJS 0.x-1.x
packages/nds-web-ember    # Ember Addon
packages/nds-web-react    # React component library
packages/nds-web-vue      # Vue component library
```


## Tagging
Tagging will be super useful for search functionality on the site.

Some common things to tag:

* platform (e.g., "web")
* framework (e.g., "react")
* platform+framework (e.g., "web-react", "mobile-react", etc.)
* concept (e.g., "accessibility", "a11y")
* technology (e.g., "html", "css", "javascript", etc.)
