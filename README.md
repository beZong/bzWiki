# bzWiki
**Markdown Wiki** - in native file system folders, with high hackability


This is the front page of my ideal **Wiki / Note Taking platform**. There might be some activities take place in somewhere else. Such as,

* retrofit some existing program
* implement in Svelte as bzWiki-sve
* implement in Vue as bzWiki-vue
* target spec in [bzWiki-spec](doc/bzWiki-spec), very likely with nodejs and a browser client

# Searching for an ideal Wiki / Note Taking platform

 Benchmark / survey, or build my own **bzWiki** ?

<!--
## ref: 
* bzWiki-vscode-crossnote.md
* todo-vscode-crossnote.md
-->

## Philosophy
* bzWiki:
  * Markdown files, in native file system folders 
  * `respect your folder structure`, loosely connect everything with limited (very less) payload files
    * => very similar to the concept of **Lolinote**
    * Spec of Lolinote 2.0 - https://github.com/visig9/lolinote-spec/blob/master/spec-2.0.md
    * Spec 1.0 - https://bitbucket.org/civalin/lolinote/wiki/Rules%20&%20Philosophy
  * aim for `hackability`
* TiddlyWiki: 
  * cook tiddlers as a set (in single HTML, or served by host), then ... [[1]](https://tiddlywiki.com/#TiddlyWiki), [[2]](https://tiddlywiki.com/#Philosophy%20of%20Tiddlers), [[3]](https://tiddlywiki.com/dev/#Microkernel%20Architecture)
> ... `structured` with links, tags, lists and macros.

> ... brought unprecedented `freedom` to everyone to keep their precious information `under their own control`.

> ... Only a small part of the TiddlyWiki is not `managed as tiddlers`,

* Evernote: 
  * organize everything (text/voice notes, drawings, attachments) for you and get them synced
* [VSCode](https://code.visualstudio.com/docs/editor/whyvscode): 
  * Edit, build, and debug with ease.
  * Make it your own - `Customize every feature`

## Scoring
  * (5) best
  * ...
  * (1) poor
  * (0) negative

## File Format / Storage: 
* bzWiki: Markdown files, in native file system folders 
* (3.5) TiddlyWiki
  * single html (in browser), or 
  * [wiki folder](https://tiddlywiki.com/#TiddlyWikiFolders) (with node.js backend)
  * official [markdown plugin](https://tiddlywiki.com/#Markdown%20Plugin)
* (2) Evernote: proprietary database, only 2-layer folder
* (3.5) VSCode: as source code editor, `respect your folder structure`

## Usability: UI / Sync / sharing
* bzWiki: try to be fusion of Evernote and TiddlyWiki
* (3) TiddlyWiki: someone like, while others don't
* (4) Evernote: 
  * Handy with `PC / mobile sync`, and `sharable link`
  * only one main window, not good for massive search / browsing
* (3) VSCode: most for technical people, not for wiki

## Hackability / Plugin / Macro
* bzWiki: target to be as good as TiddlyWiki
* (4) TiddlyWiki: `first class hackability`
* (1) Evernote: by import / export *.enex (XML), or Evernote API
* (3) VSCode: `rich extension library`, but not easy for beginner to code his own extension

## Potential Candidate
Years ago, my previous attempt to create
* (2015) [Hierarchical Note Taking App](https://github.com/beZong/beZong/tree/master/pic) -- [[1](https://github.com/Eucaly/bezongmemo)]  [[2](https://github.com/jbaron/cats/issues/141)]
* (2016) [Markdown viewer](https://github.com/beZong/bZmd)

Today's technology (2020) tends to bring me an existing program, or even to build my own.

### Major criterions
  * Markdown files, in native file system folders
  * File browsing / tree view / fulltext search
  * Easy to customize / extend => function and markdown syntax
  * not too heavy
### vscode-crossnote
  * TypeScript - [further details](https://github.com/0xGG/vscode-crossnote/issues/27)
### [hakanu/pervane](https://github.com/hakanu/pervane)
  * Plain text file based note taking and knowledge base building tool, markdown editor, simple browser IDE.
  * py (Flask server), js, md - [further details](https://github.com/hakanu/pervane/issues/98)
### [fiatjaf/coisas](https://github.com/fiatjaf/coisas)
  * client-side CMS for editing GitHub Markdown (and other) files
### Vue framework
* [docsify](https://docsify.js.org/#/)
  * ... generates your documentation website on the fly. ... smartly loads and parses your Markdown files and displays them
  * vue, marked, plugin
### Svelte framework
* [Sapper](https://sapper.svelte.dev/) - application framework powered by Svelte — build bigger apps with a smaller footprint
* SvelteWeb
  * creating Svelte powered websites using markdown - [raguay/SvelteGithubSiteTemplate](https://github.com/raguay/SvelteGithubSiteTemplate)
  * tutorial - https://dev.to/raguay/using-the-svelte-github-website-template-1ca1
* Markdown preprocessor for Svelte. https://mdsvex.com/ 
* Write Svelte components in markdown syntax - https://alexxnb.github.io/svelte-preprocess-markdown/  