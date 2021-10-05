# amp-blog-theme

A simple blog theme supports for [AMP](https://amp.dev/).

## Features

- [x] AMP Page
- [x] Google Analytics
- [x] Google AdSense
- [ ] Latex (Math) Support

## Example Configuration

**config.yaml**

```yaml
baseURL: 'https://your-site.com/'
languageCode: 'en-us'
defaultContentLanguage: en
title: 'Blog | authorName'
theme: 'amp-blog-theme'
author: 
  name: 'authorName'
  email: name@example.com

markup:
  defaultMarkdownHandler: goldmark
  goldmark:
    extensions:
      definitionList: true
      footnote: true
      linkify: true
      strikethrough: true
      table: true
      taskList: true
      typographer: true
    parser:
      attribute:
        block: false
        title: true
      autoHeadingID: true
      autoHeadingIDType: github
    renderer:
      hardWraps: false
      unsafe: false
      xhtml: false
  highlight:
    anchorLineNos: false
    codeFences: true
    guessSyntax: false
    hl_Lines: ""
    lineAnchors: ""
    lineNoStart: 1
    lineNos: false
    lineNumbersInTable: true
    noClasses: true
    style: manni
    tabWidth: 2
  tableOfContents:
    endLevel: 3
    ordered: false
    startLevel: 2
```
