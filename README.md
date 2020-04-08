# 🧠 Brain

*aka Markdown Notes with Atom*

> Healthy reaction, constructive reaction, can start from a wrong idea clearly defined, whereas mere muddle effects nothing whatever
>—Ezra Pound

![Beanie](assets/README-e75486d8.gif)

No peeking!

But really, I use this setup for note taking and thinking with [Atom](https://atom.io/).
I've kept the actual content out but am sharing my setup for its
improvement and/or your amusement.

## ⚙️ Setup

I use `asdf` for managing `node` versions.  I run this repo on `v6.3.1` but
I imagine it works on many others.

Assuming you have a reliable `node` setup and [brew](https://brew.sh/) installed (or are a nix user who has read far past this already)...

```bash
npm install
brew install atom
apm install browser-plus@0.0.98 busy-signal@2.0.1 clipboard-plus@0.5.1 \
  date@2.6.0 file-icons@2.1.39 git-plus@8.7.1 hey-pane@1.2.0 \
  highlight-colors@0.9.0 highlight-line@0.12.0 highlight-selected@0.17.0 \
  intentions@1.1.5 link-helper@0.2.0 linkist@1.3.1 lint-scroll-marker@0.3.0 \
  linter@2.3.1 linter-markdown@5.2.11 linter-ui-default@1.8.1 \
  markdown-fold@0.3.0 markdown-image-assistant@0.2.2 \
  markdown-preview-enhanced@0.17.7 markdown-toc@0.4.2 prettier-atom@0.58.2 \
  scroll-marker@0.3.2 tree-view-git-status@1.5.2 wordcount@3.1.0 \
  hyperclick path-hyperclick hyperlink-hyperclick atomic-management
```

## Usage
**🗄 File structure**
I use directories for my core interests:

```
🛒 ankauf
🔑 backups
🧪 biochem
💼 biz
🔍 catalog
📙 cheatsheets
👪 chronicle
🚘 drive
🏠 dwell
🥙 eat
🗺 explore
🇸🇦 faeal
🐕 fauna
🇵🇹 fazer
🎩 floss
🤠 fort
👾 hack
😂 haha
💡 ideas
📈 invest
⚖️ law
🎧 listen
👀 look
🇩🇪 machen
💾 manuals
📓 notes
🌱 plant
📚 read
🎙 record
🇯🇵 suru
💊 thrive
🌊 torrent
📍 ux
🏺 verkauf
👝 wallet
🍿 watch
⚡️ wire
✍️ write
🐼 zuo
```

NOTE: Using emoji in directories can cause problems for your command line interface.  You have been warned.  But if you are going to go for it and are so foolhardy as to lead with them, you can still sort them alphabetically...

```sh
ls | sort -k2
```

Within each of these, I keep a `CHANGELOG.md` and a `TODO.md`.  I sporadically sequester large or antiquated stuff into an `./archive` subdirectory for punting off to an external drive.

**🏙 Images**

Drop an image into the editor, and Atom will copy it to the `assets` folder and
generate the appropriate markdown.

**⌨️ Hot Keys**

Basic hot keys

Command | Action
:-:|:-:
`ALT`-`CMD`-`t`| Open terminal
`CMD`-`p`| Project file search
`CMD`-`P`| Command palette (use to add date)
`CMD`-`,`| Settings

Markdown and Pane hot keys

Command | Action
:-:|:-:
`CTRL`-`SHIFT`-`m`| Markdown preview
`CMD`-`K`| Pane toggle
`CTRL`-`(`| Git pane
`CMD`-`k`,`CMD`-`b`| Toggle tree

Navigation hot keys

Command | Action
:-:|:-:
`CTRL`-`l`| Create a ^tag^  
`CTRL`-`ALT`-`l`| Jump to next ^tag^  
`CTRL`-`{`| Fold all  
`OPT`-`CMD`-`]`| Unfold this  
`OPT`-`CMD`-`}`| Unfold all

**📠 CLI**

I use [fish](https://fishshell.com/) for my CLI and I use the following abbreviation to randomly pick a
directory when I'm looking for something to do.

```fish
abbr cdr (find ./ -type d -d 1 | shuf -n 1)
```
