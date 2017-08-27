# hugo-material-theme

hugo-material-theme is a material design hugo theme for [my website](https://mosko.tokyo).

> Material Design is a unified system that combines theory, resources, and tools for crafting digital experiences. ([Material Design](https://material.io/))

In addition to the original material design, [font awesome](http://fontawesome.io/) and [KaTeX](https://github.com/Khan/KaTeX) is used.

## installation

At hugo's project root,

```bash
git clone https://github.com/moskomule/hugo-material-theme
hugo server -t hugo-material-theme
```

For syntax highlighting, you need

```bash
pip install Pygents
```

## configurations

```toml
baseurl = "https://foobar.com/"
languageCode = "ja"
title = "foobar log"
theme = "hugo-material-theme"
pygmentsuseclasses = true
DefaultContentLanguage = "ja"

[Params]
author = "Ὅμηρος"
aboutMe = "Ποιητης ειμι"
showsRSS = true
copyright = "Written by Homer"

[[Params.social]]
  medium = "twitter"
  icon = "twitter"
  link = "https://twitter.com/homerus"

[[Params.topics]]
  topic = "poem"
  url = "poem"
  pic = "img/poet.jpg"
  alt = "articles on poems"
```

## todo

- [ ] multilingual
- [ ] flexible content sidebar
