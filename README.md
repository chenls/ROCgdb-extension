# rocgdb-extension README

Extension for Theai and VSCode to use ROCGDB.

## Features

Displays Agents, Queues, Dispatches, Lanes information when executing GPU code with the ROCm environment.

## Usage requirements

You need a [ROCm environment](https://github.com/RadeonOpenCompute/ROCm) with [ROCgdb](https://github.com/ROCm-Developer-Tools/ROCgdb) already installed.
In order to run this plugin, you will also need either [Visual Studio Code](https://github.com/Microsoft/vscode) or [Theia IDE](https://github.com/eclipse-theia/theia) with debugger support and vscode plugin support.

## Usage instructions

1. Download the VSIX from the releases or follow the instructions to compile from source <br />
Then from Visual Studio Code or Theia interface:
2. Extensions (Ctrl+Shift+X)
3. `...` in the upper right hand corner
4. `Install from VSIX...`
5. Select the VSIX in the file explorer

## Compile requirements

- [vsce](https://github.com/microsoft/vscode-vsce) : `npm install -g vsce`
- [Node.js](https://nodejs.org/en/) at least `14.x.x`

## Compile instructions

```
npm install
vsce package
```

## Known Issues

- Breakpoints will not show in the kernel function before loading the code object.

## Release Notes

### 0.1.0

Initial release.
