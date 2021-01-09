<!-- markdownlint-disable MD033 MD041 -->
<!-- Generated by .automation/build.py, please do not update manually -->

<div align="center">
  <a href="https://prettier.io/" target="blank" title="Visit linter Web Site">
    <img src="https://github.com/standard/standard/raw/master/sticker.png" alt="prettier" height="150px" class="megalinter-banner">
  </a>
</div>

## prettier documentation

- Visit [Official Web Site](https://prettier.io/){target=_blank}
- See [How to configure prettier rules](https://prettier.io/docs/en/configuration.html){target=_blank}
- See [How to disable prettier rules in files](https://prettier.io/docs/en/ignore.html#javascript){target=_blank}
- See [Index of problems detected by prettier](https://prettier.io/docs/en/options.html){target=_blank}

[![prettier - GitHub](https://gh-card.dev/repos/prettier/prettier.svg?fullname=)](https://github.com/prettier/prettier){target=_blank}

## Configuration in Mega-Linter

- Enable prettier by adding `JAVASCRIPT_PRETTIER` in [ENABLE_LINTERS variable](https://nvuillam.github.io/mega-linter/configuration/#activation-and-deactivation)
- Disable prettier by adding `JAVASCRIPT_PRETTIER` in [DISABLE_LINTERS variable](https://nvuillam.github.io/mega-linter/configuration/#activation-and-deactivation)

- Enable **auto-fixes** by adding `JAVASCRIPT_PRETTIER` in [APPLY_FIXES variable](https://nvuillam.github.io/mega-linter/configuration/#apply-fixes)

| Variable | Description | Default value |
| ----------------- | -------------- | -------------- |
| JAVASCRIPT_DEFAULT_STYLE | For prettier to be active, JAVASCRIPT_DEFAULT_STYLE must be `prettier` | `standard` |
| JAVASCRIPT_PRETTIER_ARGUMENTS | User custom arguments to add in linter CLI call<br/>Ex: `-s --foo "bar"` |  |
| JAVASCRIPT_PRETTIER_FILTER_REGEX_INCLUDE | Custom regex including filter<br/>Ex: `(src|lib)` | Include every file |
| JAVASCRIPT_PRETTIER_FILTER_REGEX_EXCLUDE | Custom regex excluding filter<br/>Ex: `(test|examples)` | Exclude no file |
| JAVASCRIPT_PRETTIER_FILE_EXTENSIONS | Allowed file extensions. `"*"` matches any extension, `""` matches empty extension. Empty list excludes all files<br/>Ex: `[".py", ""]` | `[".js"]` |
| JAVASCRIPT_PRETTIER_FILE_NAMES_REGEX | File name regex filters. Regular expression list for filtering files by their base names using regex full match. Empty list includes all files<br/>Ex: `["Dockerfile(-.+)?", "Jenkinsfile"]` | Include every file |
| JAVASCRIPT_PRETTIER_CONFIG_FILE | prettier configuration file name</br>Use `LINTER_DEFAULT` to let the linter find it | `.prettierrc.json` |
| JAVASCRIPT_PRETTIER_RULES_PATH | Path where to find linter configuration file | Workspace folder, then Mega-Linter default rules |
| JAVASCRIPT_PRETTIER_DISABLE_ERRORS | Run linter but disable crash if errors found | `false` |

## IDE Integration

Use prettier in your favorite IDE to catch errors before Mega-Linter !

| <!-- --> | IDE | Extension Name | Install |
| :--: | ----------------- | -------------- | :------: |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/atom.ico" alt="" height="32px" class="megalinter-icon"></a> | [Atom](https://atom.io/) | [prettier-atom](https://github.com/prettier/prettier-atom) | [Visit Web Site](https://github.com/prettier/prettier-atom){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/atom.ico" alt="" height="32px" class="megalinter-icon"></a> | [Atom](https://atom.io/) | [atom-mprettier](https://github.com/t9md/atom-mprettier) | [Visit Web Site](https://github.com/t9md/atom-mprettier){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/atom.ico" alt="" height="32px" class="megalinter-icon"></a> | [Atom](https://atom.io/) | [atom-miniprettier](https://github.com/duailibe/atom-miniprettier) | [Visit Web Site](https://github.com/duailibe/atom-miniprettier){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/emacs.ico" alt="" height="32px" class="megalinter-icon"></a> | [Emacs](https://www.gnu.org/software/emacs/) | [prettier-emacs](https://github.com/prettier/prettier-emacs) | [Visit Web Site](https://github.com/prettier/prettier-emacs){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/emacs.ico" alt="" height="32px" class="megalinter-icon"></a> | [Emacs](https://www.gnu.org/software/emacs/) | [prettier.el](https://github.com/jscheid/prettier.el) | [Visit Web Site](https://github.com/jscheid/prettier.el){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/emacs.ico" alt="" height="32px" class="megalinter-icon"></a> | [Emacs](https://www.gnu.org/software/emacs/) | [apheleia](https://github.com/raxod502/apheleia) | [Visit Web Site](https://github.com/raxod502/apheleia){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/idea.ico" alt="" height="32px" class="megalinter-icon"></a> | [IDEA](https://www.jetbrains.com/products.html#type=ide) | [native support](https://prettier.io/docs/en/webstorm.html) | [Visit Web Site](https://prettier.io/docs/en/webstorm.html){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/sublime.ico" alt="" height="32px" class="megalinter-icon"></a> | [Sublime Text](https://www.sublimetext.com/) | [JsPrettier](https://packagecontrol.io/packages/JsPrettier) | [Visit Web Site](https://packagecontrol.io/packages/JsPrettier){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/vim.ico" alt="" height="32px" class="megalinter-icon"></a> | [vim](https://www.vim.org/) | [vim-prettier](https://github.com/prettier/vim-prettier) | [Visit Web Site](https://github.com/prettier/vim-prettier){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/default.ico" alt="" height="32px" class="megalinter-icon"></a> | visual_studio | [JavaScriptPrettier](https://github.com/madskristensen/JavaScriptPrettier) | [Visit Web Site](https://github.com/madskristensen/JavaScriptPrettier){target=_blank} |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/vscode.ico" alt="" height="32px" class="megalinter-icon"></a> | [Visual Studio Code](https://code.visualstudio.com/) | [prettier-vscode](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) | [![Install in VsCode](https://github.com/nvuillam/mega-linter/raw/master/docs/assets/images/btn_install_vscode.png)](vscode:extension/esbenp.prettier-vscode){target=_blank} |

## Mega-Linter Flavours

This linter is available in the following flavours

| <!-- --> | Flavor | Description | Embedded linters | Info |
| :------: | :----- | :---------- | :--------------: | ---: |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/images/mega-linter-square.png" alt="" height="32px" class="megalinter-icon"></a> | [all](https://nvuillam.github.io/mega-linter/supported-linters/) | Default Mega-Linter Flavor | 78 | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter) |
| <img src="https://github.com/nvuillam/mega-linter/raw/master/docs/assets/icons/javascript.ico" alt="" height="32px" class="megalinter-icon"></a> | [javascript](https://nvuillam.github.io/mega-linter/flavors/javascript/) | Optimized for JAVASCRIPT or TYPESCRIPT based projects | 42 | ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/nvuillam/mega-linter-javascript/v4) ![Docker Pulls](https://img.shields.io/docker/pulls/nvuillam/mega-linter-javascript) |

## Behind the scenes

### How are identified applicable files

- File extensions: `.js`

<!-- markdownlint-disable -->
<!-- /* cSpell:disable */ -->

### Example calls

```shell
prettier --check myfile.js
```

```shell
prettier --config .prettierrc.json --check myfile.js
```

```shell
prettier --config .prettierrc.json myfile.js
```


### Installation on mega-linter Docker image

- NPM packages (node.js):
  - [prettier](https://www.npmjs.com/package/prettier)