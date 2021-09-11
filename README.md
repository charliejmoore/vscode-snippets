# vscode-snippets

[vscode-snippets](https://github.com/charliejmoore/vscode-snippets) is a collection of useful [snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets) for [VS Code](https://code.visualstudio.com/).

I created many of these snippets with this helpful [snippet generator](https://snippet-generator.app/) tool.

## Contents

- [TypeScript snippets](https://github.com/charliejmoore/vscode-snippets/blob/master/typescript.json)
- [Markdown snippets](https://github.com/charliejmoore/vscode-snippets/blob/master/markdown.json)
- [HTML snippets](https://github.com/charliejmoore/vscode-snippets/blob/master/html.json)
- [SCSS snippets](https://github.com/charliejmoore/vscode-snippets/blob/master/scss.json)

## Usage

To add any of these snippets to your own VS Code editor:
  1. Open the [Command Palette](https://code.visualstudio.com/docs/getstarted/userinterface#_command-palette) (`cmd` + `shift` + `p` on Mac, `ctrl` + `shift` + `p` on Windows).
  2. Search for and select `Preferences: Configure User Snippets`.
  3. A list of languages will appear and you can browse or search for the language of the snippet you want to add. Select that option.
  4. A `<language_name_or_extension>.json` file should show up.
  5. Between the top level set of curly braces, (e.g., `{ }`), copy-paste the snippets you want to add. **
  6. Save your file and your new snippets will be available to use when you have a file of the corresponding language type open.

## Troubleshooting

##### Conflicting Settings

There are various [user settings](https://code.visualstudio.com/docs/getstarted/settings) that may interfere with editor suggestions behavior (which can include snippets). Check out your `settings.json` (global and/or workspace-level if applicable) to see if you have anything configured that might suppress editor suggestions.

To quickly access your `settings.json`, open the Command Palette (`cmd` + `shift` + `p` on Mac, `ctrl` + `shift` + `p` on Windows) and search for `settings` and select `Preferences: Open Settings (JSON)`. You may be able to diagnose problems through the UI-based settings page if you prefer to work with that.

##### Is Your Snippet File Valid JSON?

Double check that your snippet file is valid `json` or [`jsonc`](https://code.visualstudio.com/docs/languages/json#_json-with-comments) (e.g., make sure each snippet entry is separated from the next snippet with a comma, etc).

It can be frustratingly difficult to spot an issue with `json`, so I find this online [JSON validation tool](https://jsonlint.com/) to be super helpful in diagnosing problems with snippets and `settings.json`. Note: the validation tool will complain about comments, so if you are using `jsonc`, keep that in mind.

##### Submit an Issue

There might also be something off with my snippets, so feel free to [submit an Issue](https://github.com/charliejmoore/vscode-snippets/issues) if you'd like me to check it out!
