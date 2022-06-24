# rss extended abstract landing page
- stylesheet based on this one: https://gist.github.com/killercup/5917178
- template based on the pandoc default one

## basic usage:
- install pandoc (latest version from https://github.com/jgm/pandoc/releases/tag/2.18)
- edit index.md to your liking. for youtube videos use the custom divs.
- run `./build.sh` to generate index.html
- manually deploy `index.html` and `static` folder (e.g. to gh pages) or run `python3 -m http.server` for previewing the site.
