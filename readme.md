![front](https://user-images.githubusercontent.com/675812/236014786-d399c38d-1017-453a-a7c8-ad023f05319b.jpg)

Keepcalm, a color theme for Visual Studio Code focused on software development.

https://marketplace.visualstudio.com/items?itemName=sgmonda.keepcalm-theme

## Contributing

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

To build a shareable VSIX file, after updating the `version` field in the `package.json` file, run the following in the main window:

- `npm run build`

Now you can share the VSIX file and install it in any computer:

- ⌘⇧P
- Extensions: install from VSIX...

### Publishing

Create an access token in Azure DevOps:

- https://dev.azure.com/sgmonda

Create a publisher in VSCode marketplace:

- https://marketplace.visualstudio.com/manage

Prepare VSCE CLI

- `npm run login`
- Enter the access token

After changes, update the `package.json` version and run:

```bash
$ npm run build
$ git add . && git commit -am '...'
$ npm run publish
```
