# OpenApi Snippets

## Usage

currently supported snippets:
- `pathget`
- `pathpost`
- `pathput`
- `schemaObject`
- `propertyObject`

JSON files are being validated according to their respective usage (e.g. Schema Objects). For schema specifications, see [OpenApi Specification v3 ](https://raw.githubusercontent.com/OAI/OpenAPI-Specification/master/schemas/v3.0/schema.json)

For IntelliSense to validate the files, filenames have to match their respective schema:
Object Type|filename
--- |---
schemaObject| \*-schema.json
Path Item|\*-path.json

You can navigate through predefined anchor points with TAB key. This only works right after inserting a snippet. 

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
