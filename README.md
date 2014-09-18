## Overview

[Harp Boilerplate](http://harpjs.com/) which uses the ***css styling*** from the [github-markdown-css project](https://github.com/sindresorhus/github-markdown-css).  

Helpful for viewing/testing [Github Flavored Markdown](https://help.github.com/articles/github-flavored-markdown).

## Getting Started

Read the [Harp Quick Start Guide](http://harpjs.com/docs/quick-start) to install and get started with [Harp](http://harpjs.com/).

To use this project as a boilerplate see the [docs](http://harpjs.com/docs/environment/init).

**Example:**

```
harp init docs --boilerplate techstreams/harp-github-markdown
harp server docs
```

Edit the markdown in the [public/index.md](public/index.md) file and save.  *Edit the [harp.json](harp.json) file to change the title.*

Visit [localhost:9000](http://localhost:9000) in your browser to view.



**Note**

This boilerplate uses `ejs` for the [layout template](public/_layout.ejs).   If you want to use `jade`, substitute the following code in [public/_layout.ejs](public/_layout.ejs) and rename it to `_layout.jade`

**_layout.jade**

```
!!! 5
html
  head
    meta(charset='utf-8')
    meta(name='viewport', content='width=device-width, initial-scale=1, minimal-ui')
    title
    link(rel='stylesheet', href='css/github-markdown.css')
    style.
      body {
      min-width: 200px;
      max-width: 790px;
      margin: 0 auto;
      padding: 30px;
      }
  body
    article.markdown-body
      != yield
```


## Credits

* [Sindre Sorhus](http://sindresorhus.com) for the [CSS](https://github.com/sindresorhus/github-markdown-css)
* [Harp](http://harpjs.com/) for the web server


## License

[CSS](public/css/github-markdown.css) is licensed MIT © [Sindre Sorhus](http://sindresorhus.com)

Project is licensed MIT © [Laura Taylor](https://github.com/techstreams)
