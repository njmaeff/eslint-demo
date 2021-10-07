# ESLint demo

ESLint is a lint checker for javascript. 

## Using Online
You can use the tool online at [https://eslint.org/demo](https://eslint.org/demo) to test your code and play with configuration options. There is an option at the bottom of the screen to download the configuration file afterward.

## Use Programmatically

1. Install NodeJS version 14 [https://nodejs.org/en/download/](https://nodejs.org/en/download/).

1. If you are on Mac or Linux, you will need to update where NodeJS stores packages using the command line. Follow the instructions here [https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally) to change the location. Below is a script you can run in the terminal.

    ```bash
    npm config set prefix '~/.npm-global'
    echo 'export PATH=~/.npm-global/bin:$PATH' >> ~/.profile
    source ~/.profile
    ```

1. Update npm (Node Package Manager) on your computer.

    ```bash
    npm install -g npm@latest
    ```

1. Install the `eslint` package globally.

    ```bash
    npm instal -g eslint
    ```

1. Install the `ESLint` vscode extension. You can search for the extension using this identifier `dbaeumer.vscode-eslint`. Microsoft maintains this extension, so it should be pretty safe.

### Project Structure

Create a`.eslintrc.json` or `.eslintrc.js` in your root directory where you plan on storing your project files.

If set up correctly, you will see the red squiggly lines in your editor, and when you hover over the error, it should tell you if it is a lint error. ESLint can fix specific errors automatically, for example, missing semi-colons.

You can run `eslint` on the command line.

```bash
# check files in the current directory
eslint .
```

```bash
# check files in the current directory and fix if possible.
eslint --fix .
```

## About
ESLint is one of the most popular lint checkers and has a solid open source community. The source code is on [GitHub](https://github.com/eslint/eslint).

