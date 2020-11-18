# Solar Theme for Hugo - Gruvbox edit

## Edits summary
Those edits were designed to customize the original theme into what backs [my blog][retroactive]

- Reworked the style to use [gruvbox] as a theme instead.
- Attempted to slim the style out by re-separating color theming from structure and removing structures I won't use.
- Tried to increase support for older browsers (understand IE) without usage of JS.
- Made the main content's slightly larger.
- More metadata in the header column, added coloring metadata where applicable.
- A taxonomy listing at the end of single's archetype.
- An entry for a Mastodon (or anything else, really) link next to Twitter has been added too.
- A duck is waiting for you at the end of the page.
- Dropped pygment syntax highlighting, uses Hugo's default Chroma instead.
- Added shortcodes because they can help.


[gruvbox]: https://github.com/morhetz/gruvbox
[retroactive]: https://retroactive.me
## Previous readme's content

A minimalistic theme for [Hugo](https://gohugo.io/) blogs, fork of
[Solar Theme for Ghost](https://github.com/mattvh/solar-theme-ghost). There is a
demo available on
[Hugos theme list](https://themes.gohugo.io/theme/solar-theme-hugo/). See the
[example config.toml](exampleSite/config.toml) for a starting point.


## Color schemes

Eiyeron: only gruvbox is available for now.

Solar offers three color schemes: (Solarized) `light`, (Solarized) `dark`
(default) and `gray`. Additionally there is a `preference` setting which
switches between `light` and `dark` according to the users preference.

## Screenshot

Eiyeron: "Screenshot machine broke", sorry.

## Additional HTML

Custom HTML can be injected just before `</head>` and `</body>` by creating a
`head.html` or `foot.html` inside the sites `layouts/partials/` folder. The
default (empty) logo can be overwritten by creating a `logo.svg` in
`static/img/`.

## Syntax Highlighting

Eiyeron: Chroma's used instead, following Hugo's recent default changes.
Syntax Highlighting should be provided by the color definition.

This theme does not bring a syntax highlighter. If you want to use
[Hugos built in one](https://gohugo.io/content-management/syntax-highlighting/),
remember to update the color scheme by
[setting pygmentsStyle](/exampleSite/config.toml#L4). The pygments style
`solarized-dark`, for example, matches the themes `dark` color scheme, while
`solarized-light` matches `light` and `solarized-dark256` works well with
`gray`.

Otherwise, if you want to use a JavaScript highlighter like
[highlight.js](https://highlightjs.org/), the necessary JavaScript can be placed
inside `static/` and get included by providing a `footer.html` as described
above.

## Installation

Same as with any other theme:

```bash
$ git clone https://github.com/bake/solar-theme-hugo.git themes/solar-theme-hugo
$ hugo server --theme solar-theme-hugo
...
```

## License

GPLv2 or higher
