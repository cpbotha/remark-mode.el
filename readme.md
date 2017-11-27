# remark-mode.el

A major mode for [remark](https://github.com/gnab/remark) - the simple, in-browser, markdown-driven slideshow tool

<img src="https://cdn.rawgit.com/torgeir/remark-mode.el/gh-pages/emacs-remark-mode.gif" />

Key bindings

- `M-n` next slide
- `M-p` prev slide
- `C-x C-s` save and reload
- `C-c C-s s` new slide
- `C-c C-s i` new incremental slide
- `C-c C-s k` kill slide
- `C-c C-s n` create note
- `C-c C-s c` connect browser

Dependencies

- [markdown-mode](https://github.com/defunkt/markdown-mode)
- node+npm
- [browser-sync](http://www.browsersync.io/) (`npm i -g browser-sync`)

Todo

- [x] Use `xdg-open` instead of `open` on linux, `open` is os x only? Or the built in `(browse-url url)`.
- [x] Show visited slide in browser (os x)
- [ ] Support custom index.html files in same folder as .remark file to allow for images
- [ ] Support moving slides around
- [ ] Don't always enter presentation mode, keep it if its on, don't turn it on
  if its off

Changelog
- 2017-11-27: v1.6.0:
Save buffer after performing slide actions (new, kill, incremental) for the
ultimate reload experience

- 2017-11-27: v1.5.0:
Handle layout: true to always show the correct slide in the browser

- 2017-11-27: v1.4.0:
Support background-image, count and layout keywords in highlighting

- 2017-11-27: v1.3.0:
Automatically visit slide under cursor in browser, not just on M-n and M-p

- 2017-11-26: v1.2.4:
Expose remark-preferred-browser as var

- 2017-11-26: v1.1.4:
Visit slide in browser on M-n and M-p

- 2017-11-26: v1.0.4:
Fix invalid syntax

- 2017-11-26: v1.0.3:
Reload on all saves, not just C-x C-s

- 2015-09-07: v1.0.0
