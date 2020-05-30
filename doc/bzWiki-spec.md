# bzWiki
 - markdown wiki / scripting / macro => kind of ... tiddlywiki, evernote
 - bzMemo / bzNote 
 
## Implementation
* markdown native format
* [[backend]] directory tree with limited (very less) payload files
* editor / preview

* preview ??
* editor ??
  * regex find / replace
### Frontend
  * browser extension
    * to hack on markdown content (not only local files)
  * served by backend
  * local html & javascript
### Backend
  * node.js local file server (http)
  * live reload
  * more file adaptors as 2nd stage

## Features
### Editor
* markdown native format
* github / gitlab / HackMD / CodiMD like operation & rendering
* (0.1) preview / edit mode ??
* User Interface
  * flexiable window
  * single / tabbed document 
    * (0.2) native by browser 
    * (advanced) auto collect tabs
  * (0.5) separate edit / preview window
  * (0.8) by wiki scripting
  * multi page / tabbed / (0.1) standlone page  [ev]
  * (0.5) window tile / cascade
* spell check  [ev] [cr]
* (0.4) drag-n-drop as title/link (or text paste ?)  [ev]
* regex find / replace
* clipboard / snippet collection
### File / Organize
* [[backend]] directory tree with limited (very less) payload files
* outline
* back / forward browsing  [ev]
* (0.1) directory tree browsing  [ev] 
  * quick move to (with folder search/suggestion) [ev]
* (0.2) multiple root directory for different realm
* smart folder / search (virtual) folder
  * [[backend]] (auto?) soft link to .md in different folder (e.g. code dev repo)
* (0.2) auto include related img
  * img / attachment side panel => hover to show
  * auto sorting
  * auto invlude (template): default / no default / top / bottom
* (0.4) thumbnail / card / list view / sorting  [ev]
* (0.6) blog archive (sync ?)
* persistent link [td]
* backup / versioning
### Sync / Sharing
* sync (with cloud drive / syncthing)  [ev]
* sharable link [ev], helped by Dropbox `or other cloud`
### Tag / meta / search
* [[backend]]/[[frontend]] full text search  [ev], link suggestion [vd] [cr]
* tagging  [ev] [td] / realm
* toc/file meta:
  * create date:
  * modify date: (auto change)
  * tag
### Hackable
* flow chart - mermaid.js 
* [[backend]] robust wiki reference (smart search missing link)
* smart link/filename conversion ??
* over/under-scroll to see some context
* Hackable (Scriptable) [td]
  * flexiable for **open source** / Bootstrap(?) [css templates](#csstemplates)
* (0.3) scripting / macro  [td]
	* embed snippet
     	* [embedmd](https://github.com/campoy/embedmd): embed code into markdown (with regexp)
	* todo list  [vd]
	* dynamic summary table
	* auto generated/update md2 files
	* local / global setting
* Import Data (digest) from Web [xl] / Web scraping
* js REPL console / data persistence
* yaml, json => data analytic
### Platform / Dependency
* phone client  [ev]

* [[frontend]]/[[backend]] version compare (review) in preview mode
  * version blame annotation by:
    * Hover tooltip ? [Link titles](https://assemble.io/docs/Cheatsheet-Markdown.html#link-titles)

[frontend]:#frontend
[backend]:#backend

### Roadmap
* version (0.x) listed as above
### Readiness
* (20%) pre-alpha (experimental)
* (40%) alpha (indev, buggy)
* (60%) pre-beta (basic function)
* (80%) beta (for daily use)
* (80%)~(100%) test/improve

### Ref:
* my previous markdown  [bZmd-new](https://github.com/beZong/bZmd), (loca)[bZmd-new](D:\Dropbox\Coding\beZong\bZmd-new\readme.md)
* [ev]:#Evernote
* [td]:#tiddlywiki
* [gh] github / gitlab
* [hk] HackMD / [cd] CodiMD -- online edit / preview
* [vd]:Vscode
* [cr] Chrome
* [xl] Excel
* [ ] stackedit
* [Markdown syntax cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

#### css_templates
  * flexiable to apply open source / Bootstrap(?) 
  * https://www.free-css.com/
  * https://templated.co/
  * https://templatemo.com/
  * http://www.oswd.org/
  * https://themewagon.com/theme_tag/open-source/
  * https://templates.silex.me/


## Benchmark
* [Note taking app comparison](https://camo.githubusercontent.com/fc5314df58aed70dccceebf0b0df6de90c3a2494/68747470733a2f2f6e6f7461626c652e6d642f7374617469632f696d616765732f636f6d70617269736f6e2e706e67)
----
### (Hackable)
### TiddlyWiki
* https://tiddlywiki.com/
* ** Highable Hackable with nothing(?)-alike
* ** locale files => single html (in browser), or [wiki folder](https://tiddlywiki.com/#TiddlyWikiFolders) (node.js backend)
* official [markdown plugin](https://tiddlywiki.com/#Markdown%20Plugin)
----
### (Edit/Preview)
### Evernote
  * https://evernote.com
  * ** sync PC / mobile
  * ** sharable link
  * -- DB, but not files, only 2-layer folder
  * -- not hackable
  * -- only one main window, not good switching among search / browsing
### Vscode
  * Visual Studio Code - https://code.visualstudio.com/
  * ** locale files
  * -- not for browsing / wiki
  * -- `no single page mode`
  * -- less feature for file meta: tag / date
### stackedit
* ttp://stackedit.io
* in browser, with
* ** multiple cloud => Google Drive, Dropbox, GitHub, Gitlab
### notable
* https://notable.md/
* -- not actual folder based / tag (meta) section in files
* -- old, 2001  v1.8.4



* [Search · note taking](https://github.com/search?l=JavaScript&o=desc&p=3&q=note+taking&s=stars&type=Repositories)
* [nicbou/markdown-notes: A note-taking application that supports Markdown, LaTeX and more. Not actively maintained.](https://github.com/nicbou/markdown-notes)
* [PolarisChen/Piece:  Less equals more. A neat and elegant app for temporary note-taking.](https://github.com/PolarisChen/Piece)
* [federicoiosue/omni-notes-desktop: Official desktop counterpart of the Android open-source note-taking app Omni Notes](https://github.com/federicoiosue/omni-notes-desktop)
* [MicroPad/MicroPad-Core: µPad (MicroPad) is an open digital note taking app](https://github.com/MicroPad/MicroPad-Core)
* [μPad | Take and organise notes for free](https://getmicropad.com/)
* [callicoder/node-easy-notes-app: A simple Note-Taking app built using Node.js, Express and Mongoose](https://github.com/callicoder/node-easy-notes-app)

## Chrome Extension - search [markdown](https://chrome.google.com/webstore/search/markdown?hl=zh-TW&_category=extensions)
* [markdown-copy](https://chrome.google.com/webstore/detail/markdown-copy/pmhimaghllfokaimpamhcbdhmogcbegh)
* [Mrkdown.io - Markdown Editor](https://chrome.google.com/webstore/detail/mrkdownio-markdown-editor/jkakmifiinaphkjndehhmochiechdimo?hl=zh-TW)
* [Markdown document renderer](https://chrome.google.com/webstore/detail/markdown-document-rendere/ccpjjnlhmfckhpjagolgbdncaiadpdpi?hl=zh-TW)
* [Markdown Viewer](https://chrome.google.com/webstore/detail/markdown-viewer/ckkdlimhmcjmikdlpkmbgfkaikojcbjk?hl=zh-TW)
* [Markdown Reader](https://chrome.google.com/webstore/detail/markdown-reader/gpoigdifkoadgajcincpilkjmejcaanc?hl=zh-TW)
* [Trello Table Markdown](https://chrome.google.com/webstore/detail/trello-table-markdown/pgifaolbebmlmfafkgngfjchfpcpndig?hl=zh-TW)
* [Markdown Menu for GitHub](https://chrome.google.com/webstore/detail/markdown-menu-for-github/jekgocfoijmbgcjejohdgmojaejofdpo?hl=zh-TW)
* [GitHub Markdown Printer](https://chrome.google.com/webstore/detail/github-markdown-printer/fehpdlpmcegfpbkgcnaleindodeegapk?hl=zh-TW)
* [Light Markdown Editor](https://chrome.google.com/webstore/detail/light-markdown-editor/efjgdajhhphockmgbagbfoaidoeinelm?hl=zh-TW)
* [Markdown Preview](https://chrome.google.com/webstore/detail/markdown-preview/hpdcheheebhjfkbdbialimlbhoopehil?hl=zh-TW)
* [Markdown Editor](https://chrome.google.com/webstore/detail/markdown-editor/ekdcaddpmiodcipjfmffhhefijpdckaf?hl=zh-TW)
* [Markdown Editor for Chrome](https://chrome.google.com/webstore/detail/markdown-editor-for-chrom/dkpldbigkfcgpamifjimiejipmodkigk?hl=zh-TW)