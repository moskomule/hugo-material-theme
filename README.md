# hugo-material-theme

hugo-material-theme is a material design hugo theme for [my website](https://mosko.tokyo).

> Material Design is a unified system that combines theory, resources, and tools for crafting digital experiences. ([Material Design](https://material.io/))

In addition to the original material design, [font awesome](http://fontawesome.io/) and [KaTeX](https://github.com/Khan/KaTeX) is used.

`hugo-material-theme` tries to support multilingual contents.

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

# shared topic
[[Params.topics]]
  topic = "poem"
  url = "poem"
  pic = "/img/poet.jpg"
  alt = "articles on poems"

[Languages]
[Languages.he]
languageName=Ἑλληνική
weight=1
visibleContents=["criticism"]
    [[Languages.he.topics]]
    topic = "criticism"
    url = "criticism"
    pic = "/img/crit.jpg"
    alt = "criticism on barbaroi"
[Languages.la]
languageName="Lingua Latina"
weight=2
visibleContents=["history"]
    [[Languages.la.topics]]
    topic = "hisotry"
    url = "history"
    pic = "/img/crit.jpg"
    alt = "hisotry of the Roman Empire"
```

## todo

- [ ] remove hard coded contents
- [ ] multilingual
- [ ] flexible content sidebar
