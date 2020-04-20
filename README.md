# OpenApi Snippets

## Usage

### snippets

currently supported snippets:

- `pathget`
- `pathgetparam`
- `pathpost`
- `pathput`
- `pathdelete`
- `schemaObject`
- `propertyObject`

### validation

JSON files are being validated according to their respective usage (e.g. Schema Objects). For schema specifications, see [OpenApi Specification v3 ](https://raw.githubusercontent.com/OAI/OpenAPI-Specification/master/schemas/v3.0/schema.json)

For IntelliSense to validate the files, filenames have to match their respective schema:
Object Type|filename
--- |---
schemaObject| \*-schema.json
Path Item|\*-path.json

You can navigate through predefined anchor points with TAB key. This only works right after inserting a snippet.

### keybindings

You can configure custom keybindings for the snippets. For this, open the keybindings.json file of VS Code (Shortcut `Ctrl+K Ctrl+S`, then click on the `Open Keyboard Shortcuts (JSON)` button in the upper right corner).
For any keybinding, use this template and edit the fields which are marked by `<<>>`:

```json
{
  "key": "<<Your desired shortcut>>",
  "command": "editor.action.insertSnippet",
  "when": "editorTextFocus",
  "args": {
    "langId": "json",
    "name": "<<Snippet prefix>>"
  }
}
```
For `name` you can use any [snippet prefix](#snippets).

## Install

You can install this extension by downloading it from the [Releases page](https://github.com/proohit/openapi-snippets/releases) and installing it via

```sh
code --install-extension openapi-snippets-EXTENSION.VERSION.NUMBER.vsix
```

## Uninstall

Uninstall it either via CLI:

```sh
code --uninstall-extension proohit.openapi-snippets
```

or via VS Code Extension Manager (default shortcut: `CTRL+Shift+X`) and then search for `@installed OpenApi Snippets`

## Update

As of now, the extension is not on VS Code Marketplace. So updating happens via uninstalling the old version and installing the updated version. You can install specific versions by uninstalling your version and installing the desired version.

## Build

For development/release, use [vsce - VS Code Extension CLI](https://code.visualstudio.com/api/working-with-extensions/publishing-extension#vsce)

```ssh
vsce package
```
