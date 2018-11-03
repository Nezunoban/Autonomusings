# Autono Theme

__`Autono`__ is a [Hugo](https://gohugo.io)'s theme inspired and derived from @spf13's [Hyde-hyde](https://github.com/htr3n/autono). 

## Breaking Changes


## Usage

### Installation

__`Autono`__ can be easily installed as many other Hugo themes:

```sh
$ cd HUGO_PROJECT

# then either clone autono
$ git clone https://github.com/Nezunoban/autono.git themes/autono

# or just add autono as a submodule
$ git submodule add https://github.com/Nezunoban/autono.git themes/autono
```

After that, choose `autono` as the main theme.

* `config.toml` 

```toml
theme = "autono"
```

* `config.yaml`

```yaml
theme : "autono"
```

That's all. You can render your site using `hugo` and see `autono` in action.

### Options

__`Autono`__ essentially inherits most of Hyde's [options](https://github.com/spf13/hyde#options). There are some extra options though

* `highlightjs = true`: use [highlight.js](https://highlightjs.org) instead of Hugo built-in support for code highlighting

  * `highlightjsstyle="highlight-style"`: only when `highlightjs = true`, please choose one of many _highlight.js_'s [styles](https://highlightjs.org/static/demo).
  * Since [v2.0.1](https://github.com/htr3n/hyde-hyde/tree/v2.0.1), highlighting for each page can be fine-tuned in the front matter, for example
    * `highlight = false`  (default `true`)
    * `highlightjslanguages = ["swift", "objectivec"]` 

* `postNavigation = true|false` (default `true`): Setting to `false` will disable the navigation _Previous Post_/ _Next Post_

* `relatedPosts = false|true` (default `false`): Setting to `true` allows related posts. Please refer [here](https://gohugo.io/content-management/related) for more details on related contents with Hugo.

* `GraphCommentId = "your-graphcomment-id"`: to use [GraphComment](https://graphcomment.com) instead of the built-in [Disqus](https://disqus.com). This option should be used exclusively with `disqusShortname = "disqus-shortname"`.

* `[params.social]`: in this section, you can set many social identities such as Twitter, Facebook, Github, Bitbucket, Gitlab, Instagram, LinkedIn, StackOverflow, Medium, Xing, Keybase.

  ```toml
  [params.social]
  	twitter = "htr3n"
  	keybase = "htr3n"
  	github = "htr3n"
  	...
  ```


### Customizations

* Most of the customisable SCSS styles in [_static-src/scss/autono_](https://github.com/Nezunoban/Autonomusings/tree/master/themes/autono/static-src/scss/autono) and Hugo templates in [_autono/layouts_](https://github.com/Nezunoban/Autonomusings/tree/master/themes/autono/blob/master/layouts) are modularised and can be altered/adapted easily.

## Portfolio

Since version 2.0+, htr3n added a portfolio page just in case. If you need it, simply add a menu section '_Portfolio_' in `config.toml` as following.

```toml
[[menu.main]]
    name = "Portfolio"
    identifier = "portfolio"
    weight = xyz
    url = "/portfolio/"
```

In the folder `content` , create a subfolder `portfolio` and use the following folder/content structure as reference.

```
$ tree portfolio
portfolio
├── _index.md
├── p1.md
├── p1.png
├── p2.md
├── p2.png
    ...
├── pn.md
└── pn.png
```

As htr3n designed the section _portfolio_ to be rendered as _list_,  `_index.md` can be used to set the title for your portfolio (you can read more about `_index.md` [here](https://gohugo.io/content-management/organization/#index-pages-index-md)). For instance, when I want to set the title of my portfolio "_Projects_", the front matter of `_index.md` will be:

```markdown
---
title: 'Projects'
---
```
The remaining of `_index.md` will be ignored.

For each project, just create a Markdown file with the following parameters in the front matter:

```markdown
---
title: "Project P1's Title"
description: "A short description"
date: '2018-01-02'
link: 'https://project-p1.com'
screenshot: 'p1.png'
layout: 'portfolio'
featured: true
---
Here is a longer summary of the project. You can write as long as you wish.
```

> __Note__:
>
> * `date` is important to sort the project chronologically
> * `layout 'portfolio'` is important as you don't want your project's page appear in the list of posts in the main page of your Web site but only in the _Portfolio_ ;)
> * `featured: true` : when you want to show a project as featured project. It is default to `false`. Note that only one project should be marked `featured: true` , otherwise, the result could be random as [the Hugo template](https://github.com/htr3n/hyde-hyde/blob/master/layouts/partials/portfolio/content.html) will take the first one.
> * The body of the Markdown file will be the summary of the project.

If you want to adjust the portfolio page to your needs, please have a look at the [main template](https://github.com/htr3n/hyde-hyde/blob/master/layouts/portfolio/list.html), that uses this [partial template](https://github.com/htr3n/hyde-hyde/blob/master/layouts/partials/portfolio/content.html) and [this SCSS style](https://github.com/htr3n/hyde-hyde/blob/master/static-src/scss/hyde-hyde/_project.scss).

## Some Screenshots

### Main page

![autono main screen](https://github.com/Nezunoban/autono/raw/master/images/main.png)

### A post

![A post in autono](https://github.com/Nezunoban/autono/raw/master/images/post.png)


## Author(s)

* Original developed by [Mark Otto](https://github.com/mdo)

* Hugo's `hyde` ported by [Steve Francia](https://github.com/spf13)

* Hugo's `Hyde-hyde` developed by [Huy Tran](https://github.com/htr3n)

## License

Open sourced under the [MIT license](LICENSE.md)
