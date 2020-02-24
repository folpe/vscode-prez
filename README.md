# VSCode Settings

## Avantages

### Historique des éditeurs de texte

- Sublime text
- Atom
- VSCode

## Extensions

| Nom                                | Nom de l'extension                    | Description                                                                                                      |
| :--------------------------------- | :------------------------------------ | :--------------------------------------------------------------------------------------------------------------- |
| **Advanced-new-file**              | patbenatar.advanced-new-file          | Create files anywhere in your workspace from the keyboard                                                        |
| **Auto close tag**                 | formulahendry.auto-close-tag          | Automatically add HTML/XML close tag, same as Visual Studio IDE or Sublime Text                                  |
| **Auto rename tag**                | formulahendry.auto-rename-tag         | Auto rename paired HTML/XML tag                                                                                  |
| **Bookmarks**                      | alefragnani.Bookmarks                 | Mark lines and jump to them                                                                                      |
| **Color Hightlight**               | naumovs.color-highlight               | Highlight web colors in your editor                                                                              |
| **Debugger for chrome**            | msjsdiag.debugger-for-chrome          | Debug your JavaScript code in the Chrome browser, or any other target that supports the Chrome Debugger protocol |
| **dotENV**                         | mikestead.dotenv                      | Support for dotenv file syntax                                                                                   |
| **ECMAScript quotes transformer**  | vilicvane.es-quotes                   | Transform quotes of ECMAScript string literals.                                                                  |
| **eslint**                         | dbaeumer.vscode-eslint                | Integrates ESLint JavaScript into VS Code                                                                        |
| **Flow langage support**           | flowtype.flow-for-vscode              | Flow support for VS Code                                                                                         |
| **Git blame**                      | waderyan.gitblame                     | See git blame information in the status bar.                                                                     |
| **github**                         | KnisterPeter.vscode-github            | Integrates github and its workflows into vscode                                                                  |
| **GraphQL for vscode**             | kumar-harsh.graphql-for-vscode        | GraphQL syntax highlighting, linting, auto-complete, and more!                                                   |
| **Javascript (es6) code snippets** | xabikos.JavaScriptSnippets            | Code snippets for JavaScript in ES6 syntax                                                                       |
| **language-stylus**                | sysoev.language-stylus                | Stylus language support                                                                                          |
| **Mardown Preview Github Styling** | Matt Bierner                          | Changes VS Code's built-in markdown preview to match Github's style                                              |
| **Markdow all in one**             | yzhang.markdown-all-in-one            | All you need to write Markdown (keyboard shortcuts, table of contents, auto preview and more)                    |
| **markdownlint**                   | DavidAnson.vscode-markdownlint        | Markdown linting and style checking for Visual Studio Code                                                       |
| **nbsp-code**                      | possan.nbsp-vscode                    | Visualizes suspicious unicode characters and trailing whitespaces                                                |
| **npm**                            | eg2.vscode-npm-script                 | npm support for VS Code                                                                                          |
| **Path Intellisense**              | christian-kohler.path-intellisense    | Visual Studio Code plugin that autocompletes filenames                                                           |
| **Prettier – code formatter**      | esbenp.prettier-vscode                | Code formatter using prettier                                                                                    |
| **Quokka.js**                      | WallabyJs.quokka-vscode               | Live Scratchpad for JavaScript                                                                                   |
| **Reactjs code snippets**          | xabikos.ReactSnippets                 | Code snippets for Reactjs development in ES6 syntax                                                              |
| **Rest client**                    | humao.rest-client                     | REST Client for Visual Studio Code                                                                               |
| **Search node_modules**            | jasonnutter.search-node-modules       | Quickly search the node_modules folder                                                                           |
| **sort-imports**                   | amatiasq.sort-imports                 | Sort ES6 imports automatically                                                                                   |
| **Sort lines**                     | Tyriar.sort-lines                     | Sorts lines of text                                                                                              |
| **Subword navigation**             | ow.vscode-subword-navigation          | The missing code navigation feature.                                                                             |
| **Typescript Hero**                | rbbit.typescript-hero                 | Additional toolings for typescript (import)                                                                      |
| **Vscode great icons**             | emmanuelbeziat.vscode-great-icons     | A big pack of icons (100+) for your files                                                                        |
| **vscode-styled-component**        | jpoissonnier.vscode-styled-components | Syntax highlighting for styled-components                                                                        |

### Installation des extensions

Command npx et/ou package.json

```javascript
npx nomDuPaquet
```

et pour être sur d'embarquer les dernières versions (ex: si extensions déjà existantes)

```javascript
npx --ignore-existing nomDuPaquet
```

## Paramètres

### Paramètres d'espace de travail

```json
{
  "eslint.workingDirectories": [
    "src"
  ],
  "search.exclude": {
    "**/.next": true
  }
}
```

### Paramètres d'utilisateur

```json
{
  // Nicer debugging
  "debug.inlineValues": true,
  // Whitespace shouldn't pollute diffs (git diff -w)
  "diffEditor.ignoreTrimWhitespace": true,
  // Font and spacing (even w/o Prettier/ESLint)
  "editor.fontFamily":
    "'Operator Mono SSm', 'Source Code Pro', Monaco, Menlo, Consolas, 'Droid Sans Mono', Inconsolata, 'Courier New', monospace",
  // For Prettier et al.
  "editor.formatOnSave": true,
  // Indent with 2 spaces!
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  // Minimaps are useless
  "editor.minimap.enabled": false,
  // Alt for click-based multi-cursor
  "editor.multiCursorModifier": "alt",
  // Don't sroll pass the last line
  "editor.scrollBeyondLastLine": false,
  // Snippets should appear above IntelliSense
  "editor.snippetSuggestions": "top",
  // A slightly fatter cursor is more visible
  "editor.cursorWidth": 3,
  // Word wrapping is usually best by default
  "editor.wordWrap": "on",
  // Hide Open Editors pane
  "explorer.openEditors.visible": 0,
  // Open any new buffer as Markdown. Super handy.
  "files.defaultLanguage": "markdown",
  // `.snap` files (Jest snapshots) should use JSX mode by default
  "files.associations": {
    "*.snap": "javascriptreact"
  },
  // Exclusions from the explorer
  "files.exclude": {
    "**/.git": true,
    "**/.DS_Store": true,
    "**/node_modules": true,
    "**/.vscode-setup-settings-merged": true
  },
  // Make diffs easier, whitespace-wise
  "files.insertFinalNewline": true,
  "files.trimTrailingWhitespace": true,
  // Only search case sensitivively for patterns that are
  // not 100% lowercase
  "search.smartCase": true,
  // Fat scrollbacks are more useful
  "terminal.integrated.scrollback": 100000,
  // Disable Preview when using Quick Open
  "workbench.editor.enablePreviewFromQuickOpen": false,
  // Show tabs again, dammit!
  "workbench.editor.showTabs": true,
  // Use cool icon theme
  "workbench.iconTheme": "vscode-great-icons",
  // Make the current tab stand out better
  "workbench.colorCustomizations": {
    "tab.activeBackground": "#08c"
  },
  // Emmet
  "emmet.includeLanguages": {
    "javascriptreact": "javascript"
  },
  "emmet.triggerExpansionOnTab": true,
  // Flow
  "flow.useNPMPackagedFlow": true,
  "javascript.validate.enable": false,
  "markdown.extension.toc.githubCompatibility": true,
  // Prettier & ESLint
  "prettier.eslintIntegration": true,
  "prettier.singleQuote": true,
  "prettier.trailingComma": "es5",
  "prettier.semi": false,
  "javascript.format.enable": false
}
```

## DEMO flow

- new file (ctrl + alt + n)
- snipets react (rsc)
- snipets es6 (imp / imd, dob)
- import sort (save)
- auto close/auto rename (create p, create span, rename span)
- nbsp (create spaces)
- bookmarks (ctrl + alt + k, lines, ctrl + alt + j)
- es Quotes transform (ctrl + shift + p > template)
- mardown all in one (create markdown file, crtl +b, alt + c)
- subword navigation (create camelCase const)
