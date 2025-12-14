# Nools Syntax Highlighting for VS Code

Syntax highlighting for the **Nools JavaScript rules engine** in Visual Studio Code.

## About

[Nools](http://noolsjs.com/) is a rules engine for javascript that implements the [Rete](https://en.wikipedia.org/wiki/Rete_algorithm) Algorithm. One application of Nools is building cognitive tutors with [CTAT](https://github.com/CMUCTAT/CTAT/wiki). 

This extension's purpose is to make writing nools more user-friendly in visual studio code. 

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
```bash
npm install
```

### 3. Package the extension
Install the VS-code extension packager (one-time):
```bash
npm install -g @vscode/vsce
```
Create the `.vsix` file:
```bash
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
```bash
code --install-extension nools-markup-0.0.1.vsix (where `0.0.1` represents the current version.)
```
### 4. Reload vscode