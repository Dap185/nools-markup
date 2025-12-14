# Nools Syntax Highlighting for VS Code

Syntax highlighting for the **Nools JavaScript rules engine** in Visual Studio Code.

This extension adds:
- JavaScript-style highlighting
- Nools keywords (`rule`, `when`, `then`, `not`, `salience`)
- Support for `.nools` files

No VS Code Marketplace account is required to use this extension.

---

##  Prerequisites

- Visual Studio Code
- Node.js (only required if you want to package a `.vsix`)
- Git

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Dap185/nools-markup.git
cd nools-markup
```

### 2. Install dependencies
```
npm install
```

### 3. Package the extension
Install the VS-code extension packager (one-time):
```
npm install -g @vscode/vsce
```
Create the `.vsix` file:
```
vsce package
```
This will generate a file, for example `nools-markup-0.0.1.vsix` (where `0.0.1` represents the current version.)

### 4. Install the extension in VS Code
code --install-extension nools-markup-0.0.1.vsix

## Making Changes
### 1. Make your changes
### 2. Build the package
```
vsce package
```
### 3. Install Updated Package
code --install-extension nools-markup-0.0.1.vsix (where `0.0.1` represents the current version.)
### 4. Reload vscode