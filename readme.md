# Keepcalm Theme for Visual Studio Code

A color theme for software development

## Development

Clone the repository and install dependencies:

- `git clone git@github.com:sgmonda/keepcalm.git`
- `npm i`

Open this project from VSCode and run

- ⌘⇧P
- Debug: Start debugging

This will open a secondary VSCode window where you can see the theme in action. Any change in the theme (first window) will be reflected in the secondary window.

To see what token a word is, from this secondary window:

- ⌘⇧P
- Developer: Inspect editor tokens and scopes

To build a shareable VSIX file, run the following in the main window:

- `npm run build`

Now you can share the VSIX file and install it in any computer:

- ⌘⇧P
- Extensions: install from VSIX...
