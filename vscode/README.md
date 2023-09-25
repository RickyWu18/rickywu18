# VS Code settings and extensions

- [VS Code settings and extensions](#vs-code-settings-and-extensions)
  - [Basic](#basic)
  - [Markdown](#markdown)
  - [Python](#python)
  - [Html, Css, Js, Ts](#html-css-js-ts)
  - [Todo tree](#todo-tree)
  - [Git, Github](#git-github)
  - [Latex](#latex)

## Basic

```json
{
  // ======== User setup ========
  // editor
  "editor.wordWrap": "on",
  "editor.minimap.enabled": false,
  "editor.tabSize": 2,
  "editor.fontSize": 16,
  "editor.fontFamily": "JetBrainsMono Nerd Font",
  "files.autoSave": "onFocusChange",
  "files.encoding": "utf8",
  "files.autoGuessEncoding": false,
  "files.trimTrailingWhitespace": true,
  "explorer.confirmDragAndDrop": false,
  "vim.smartRelativeLine": true,

  // theme
  "workbench.startupEditor": "none",
  "workbench.iconTheme": "vscode-icons",
  "workbench.colorTheme": "Default Dark+",

  // terminal
  "terminal.integrated.fontSize": 16,
  "terminal.integrated.fontFamily": "JetBrainsMono Nerd Font",
  "terminal.integrated.defaultProfile.windows": "PowerShell",

  // not important
  "vsicons.dontShowNewVersionMessage": true,
  "extensions.ignoreRecommendations": true,
}
```

Extensions:

- [vscode-icons](https://marketplace.visualstudio.com/items?itemName=vscode-icons-team.vscode-icons): `code --install-extension vscode-icons-team.vscode-icons`
- [Vim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim): `code --install-extension vscodevim.vim`
- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker): `code --install-extension streetsidesoftware.code-spell-checker`
- [indent-rainbow](https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow): `code --install-extension oderwat.indent-rainbow`

## Markdown

```json
{
  // ======== Markdown setup ========
  "[markdown]": {
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "yzhang.markdown-all-in-one",
    "editor.codeActionsOnSave": {
      "source.fixAll.markdownlint": true,
    },
  },
  "markdown.preview.scrollEditorWithPreview": true,
  "markdown.preview.scrollPreviewWithEditor": true,
}
```

Extensions:

- [Markdown All In One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one): `code --install-extension yzhang.markdown-all-in-one`
- [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint): `code --install-extension DavidAnson.vscode-markdownlint`
- [Markdown Preview Mermaid Support](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-mermaid): `code --install-extension bierner.markdown-mermaid`
- [Markdown Preview Github Styling](https://marketplace.visualstudio.com/items?itemName=bierner.markdown-preview-github-styles): `code --install-extension bierner.markdown-preview-github-styles`

## Python

```json
{
  // ======== Python setup ========
  "[python]": {
    "editor.tabSize": 4,
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "ms-python.black-formatter",
    "editor.codeActionsOnSave": {
      "source.organizeImports": true
    }
  },
  "python.terminal.activateEnvironment": true,
  "python.analysis.typeCheckingMode": "basic",
}
```

Extensions:

- [Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python): `code --install-extension ms-python.python`
- [Black](https://marketplace.visualstudio.com/items?itemName=ms-python.black-formatter): `code --install-extension ms-python.black-formatter`
- [Ruff](https://marketplace.visualstudio.com/items?itemName=charliermarsh.ruff): `code --install-extension charliermarsh.ruff`
- [autoDocstring](https://marketplace.visualstudio.com/items?itemName=njpwerner.autodocstring): `code --install-extension njpwerner.autodocstring`
- [Django](https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django): `code --install-extension batisteo.vscode-django`

## Html, Css, Js, Ts

```json
{
  // ======== Js, Ts, Html, Css setup ========
  "[html][css][javascript][typescript]": {
    "editor.tabSize": 2,
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript][javascriptreact][typescript][typescriptreact]": {
    "editor.codeActionsOnSave": {
      "source.organizeImports": true,
    }
  },
}
```

Extensions:

- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode): `code --install-extension esbenp.prettier-vscode`
- [Html CSS Support](https://marketplace.visualstudio.com/items?itemName=ecmel.vscode-html-css): `code --install-extension ecmel.vscode-html-css`
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint): `code --install-extension dbaeumer.vscode-eslint`
- [JS JSX Snippets](https://marketplace.visualstudio.com/items?itemName=skyran.js-jsx-snippets): `code --install-extension skyran.js-jsx-snippets`

## Todo tree

```json
{
  // ======== TODO tree setup ========
  "todo-tree.tree.autoRefresh": true,
  "todo-tree.highlights.customHighlight": {
    "TODO": {
      "foreground": "white", "background": "green",
      "iconColour": "lime", "icon": "check"
    },
    "BUG": {
      "foreground": "white", "background": "indianred",
      "iconColour": "crimson", "icon": "bug"
    },
    "REVIEW": {
      "foreground": "white", "background": "darkcyan",
      "iconColour": "cyan", "icon": "eye"
    },
  },
  "todo-tree.general.tags": ["TODO", "REVIEW", "BUG"],
  "todo-tree.highlights.defaultHighlight": {"type": "text-and-comment"},
  "todo-tree.regex.regex": "(%|//|#|<!--|;|/\\*|^|^[ \\t]*(-|\\d+.))\\s*($TAGS)",
}
```

Extensions:

- [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree): `code --install-extension Gruntfuggly.todo-tree`

## Git, Github

```json
{}
```

Extensions:

- [GitHub Pull Requests and Issues](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github): `code --install-extension GitHub.vscode-pull-request-github`
- [GitHub Copilot](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot): `code --install-extension GitHub.copilot`
- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens): `code --install-extension eamodio.gitlens`

## Latex

```json
{
  // ======== Latex setup ========
  "files.associations": {"*.tikz": "latex"},

  "latex-workshop.view.pdf.viewer": "tab",
  "latex-workshop.latex.autoBuild.run": "onSave",
  "latex-workshop.latex.autoClean.run": "onBuilt",
  "latex-workshop.synctex.afterBuild.enabled": true,
  "latex-workshop.synctex.synctexjs.enabled": true,
  "latex-workshop.view.pdf.external.viewer.command": "YOUR_EXTERNAL_VIEWER_PATH",
  "latex-workshop.latex.tools": [
    {
      "name": "xelatex",
      "command": "YOUR_XELATEX_COMMAND",
      "args": ["-synctex=1", "--halt-on-error", "-shell-escape", "%DOC%.tex"]
    },
    {
      "name": "pdflatex",
      "command": "YOUR_PDFLATEX_COMMAND",
      "args": ["-synctex=1", "--halt-on-error", "-file-line-error", "%DOC%"]
    },
    {
      "name": "bibtex",
      "command": "YOUR_BIBTEX_COMMAND",
      "args": ["%DOCFILE%"]
    },
    {
      "name": "biblatex",
      "command": "YOUR_BIBLATEX_COMMAND",
      "args": ["%DOCFILE%"]
    },
  ],
  "latex-workshop.latex.recipes": [
    {
      "name": "xelatex*2",
      "tools": ["xelatex", "xelatex"]
    },
    {
      "name": "xelatex->bibtex->xelatex*2",
      "tools": ["xelatex", "bibtex", "xelatex", "xelatex"]
    },
    {
      "name": "pdflatex",
      "tools": ["pdflatex"]
    },
    {
      "name": "pdflatex->bibtex->pdflatex*2",
      "tools": ["pdflatex", "bibtex", "pdflatex", "pdflatex"]
    },
  ],
  "latex-workshop.latex.clean.fileTypes": [
    "*.aux", "*.bbl", "*.blg",
    "*.idx", "*.ind", "*.lof",
    "*.lot", "*.out", "*.toc",
    "*.acn", "*.acr", "*.alg",
    "*.glg", "*.glo", "*.gls",
    "*.fls", "*.log", "*.fdb_latexmk",
    "*.snm", "*.synctex(busy)", "*.synctex.gz(busy)",
    "*.nav", "*.vrb", "*.bcf",
    "*.run.xml","*-blx.bib"
  ],
}
```

Extensions:

- [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop): `code --install-extension James-Yu.latex-workshop`
