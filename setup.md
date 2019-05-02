## Terminal environment

### ZSH

HowTo install zsh in many platforms
**macOS**

```bash
$ brew install zsh zsh-completions
```

Assuming you have Homebreww installed. If not, most versions of macOS ship zsh by default, but it’s normally an older version.

Try `zsh --version` before installing it from Homebrew. If it’s newer than 4.3.9 you might be OK. Preferably newer than or equal to 5.0.

<a href='/documents/setup.zip'>setup.zip</a>

### oh-my-zsh

[oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)

```bash
$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### iTerm2

Software that enhance the functionality of the terminal.

[Download Software](<[https://www.iterm2.com/](https://www.iterm2.com/)>)

Font inconsolata for powerline in order to see some git character.
[Link](https://github.com/powerline/fonts)

### Themes for zsh

This is a theme for zsh. You can use the link in order to install the theme.
[themes](https://github.com/robbyrussell/oh-my-zsh/wiki/Themes)
[spaceship-zsh-theme](https://github.com/denysdovhan/spaceship-zsh-theme)
[Cobalt2](https://github.com/wesbos/Cobalt2-iterm)

### NodeJS

[Link](https://nodejs.org/en/)

```bash
$ node -v
v8.6.0
$ npm -v
5.3.0
```

## VSCode

Configuration file:

```json
{
  "editor.fontFamily": "Operator Mono",
  "editor.formatOnPaste": true,
  "editor.tabSize": 2,
  "editor.insertSpaces": true,
  "editor.detectIndentation": true
}
```

### plugins

List of plugins.

[ES7 React/Redux/React-Native/JS snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
[ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
[Markdown Preview Enhanced](https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced)
[markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint)

### Themes

[new moon](https://taniarascia.github.io/new-moon/)
[material-theme](https://material-theme.site/)
[citylights](http://citylights.xyz/)

#### ESLint

[Link](<[https://eslint.org](https://eslint.org)>)

In order to use eslint we need to install eslint package. you should have installed `node`

```bash
npm install -g eslint
```

And we will need to create the configuration file `.eslintrc.json` in your project folder.
In this file we will set up all the options and rules that we will apply to our project.

Because we don’t want to review all the rules available we will install some differents packages with differents rules applied.

#### `eslintrc.json`

```json
{}
```

## Git

### `.gitconfig`

in your route folder

```batch
# This is Git's per-user configuration file.

[user]
  name = <your name here>
  email = <write her your email without <> >
[core]
  excludesfile = /Users/<your user name>/.gitignore_global
  editor = nano
  pager = cat
[alias]
  lg1 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all
  lg2 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)' --all
  lg = !"git lg1"
```

### .gitignore_global

```txt
*~
.DS_Store
*.orig
settings.json
/node_modules/
.env
```
