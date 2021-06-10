# team-dang-productivity

A little repo with some handy productivity saving configuration and tools for working on Lob's Vue repos.

## Editor
[VSCode](https://code.visualstudio.com/) is my personal IDE of choice. This repo assumes that you are using that IDE. If you're not, that's cool! All IDEs are welcome, I just know VSCode best and can offer tips and tricks for it 🤗

## Extensions
### General
- [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur): Vue tooling for VS Code.
- [Bracket Pair Colorizer 2](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer-2): This extension allows matching brackets to be identified with colours. The user can define which tokens to match, and which colours to use.
- [Peacock](https://marketplace.visualstudio.com/items?itemName=johnpapa.vscode-peacock): Subtly change the color of your Visual Studio Code workspace. Ideal when you have multiple VS Code instances, use VS Live Share, or use VS Code's Remote features, and you want to quickly identify your editor.
- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag): Automatically rename paired HTML/XML tag, same as Visual Studio IDE does.

### Testing
- [Switch to test](https://marketplace.visualstudio.com/items?itemName=eskimoblood.create-test): This extension will open the coresponding test file for the opened source file. If the file not exists, it will create a new one.
### Linting
- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint): Integrates ESLint into VS Code.

### Settings
Please see [settings.json](settings.json) for info on how to configure these extensions for productivity.

- Auto save files when you blur or navigate away from them
- Custom colors for matching brackets, parentheses, etc (choose your own colors!)
- Lint and autoformat files on save (this is the bulk of the settings in this file)
- Auto create *.spec.js files in the correct location when you use the `createTest` command (Cmd + Shift + P > Create test or you can set up a custom keyboard shortcut)

## Snippets
[Code snippets](https://code.visualstudio.com/docs/editor/userdefinedsnippets) are templates that make it easier to enter repeating code patterns, such as loops or conditional-statements.

To add new snippets, go to Code > Preferences > User snippets and then choose the language and file type you want this snippet available in.

Below you'll find my most used snippets for DANG projects.

### Vue
- [Component](vue-component-snippet.json): boilerplate for a Vue component that is available when you start typing `component` 
- [Spec](vue-spec-snippet.json): boilerplate for a spec file for a Vue component that is available when you start typing `spec`
- [Story](vue-story-snippet.json): boilerplat for a Storybook story for a Vue component that is available when you start typing `story`
### Javascript
- [Debugging](debugging-snippets.json) snippets
  - `db` will get you a `debugger` statement
  - `log` will get you a console log with your cursor ready to start typing your label and output
- [Jest](jest-snippets.json) snippets
  - `describe` will get you a jest describe block with your cursor ready to start typing your `it` blocks
  - `it` will get you a jest it block with your cursor ready to start typing your assertions
  - `before` will get you a jest beforeEach block with your cursor ready to start typing your setup code
