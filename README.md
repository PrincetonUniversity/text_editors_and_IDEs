# Text Editors and Integrated Development Environments (IDEs)

One needs to use a tool to enter and modify source code. On this page we discuss the different tools and their pros and cons.

## Command-Line Text Editors

### emacs

To start emacs on a Research Computing system:

```
$ emacs
```

`emacs` can be used for many tasks beyond text editing. It can be configured to mimic an IDE. Some find that a finely-tuned `emacs` configuration can outpace any IDE for software engineering. Visit the [emacs](https://www.gnu.org/software/emacs/) website. `emacs` takes some time to learn.

### nano

To start emacs on a Research Computing system:

```
$ nano
```

`nano` is easy to learn.

### vim

To start emacs on a Research Computing system:

```
$ vim
```

`vim` has a scripting language that allows for plugin-like extensions to enable IDE behavior, syntax highlighting, colorization as well as other advanced features. With `vim` and `emacs` you keep your hands on the keyboard and rarely use the mouse. Some find this helpful not only for productivity but to reduce repetitive strain injury (RSI) such as carpal tunnel syndrome. `vim` takes some time to learn. Visit the [vim](https://www.vim.org/) website.

In January 2025, look for the Wintersession workshop [Mastering vim: Edit as Fast as You Think](https://github.com/troycomi/intermediate-vim).

### neovim

[Neovim](https://neovim.io/) is a fork on vim with refactoring and modernizing the codebase and feature set. See an overview of Neovim on [YouTube](https://www.youtube.com/watch?v=c4OyfL5o7DU) in 100 seconds. Plugins in Neovim are written in Lua. [LazyVim](https://www.lazyvim.org/) is a Neovim setup powered by `lazy.nvim` to make it easy to customize and extend your config. Read about [Vim versus Neovim](https://lazyvim-ambitious-devs.phillips.codes/course/chapter-1/).

Neovim offers these benefits:

- plugins written in Lua  
- built-in language server protocol (LSP) for code completion
- scriptable terminal emulator
- telescope: a fuzzy file finder plugin
- treesitter for syntax highlighting

On the Research Computing clusters, you should build Neovim from source so that you can use the latest version. To use version 0.9.5, run these commands: 

```bash
$ wget https://github.com/neovim/neovim/releases/download/v0.9.5/nvim-linux64.tar.gz
$ tar -C . -xzf nvim-linux64.tar.gz
$ cd bin
$ ./nvim
```

## IDEs

What is an IDE? An integrated development environment (IDE) is a software application that helps programmers develop software code efficiently. It increases developer productivity by combining capabilities such as software editing, building, testing, and packaging in an easy-to-use application.

### VS Code

[Visual Studio Code](https://code.visualstudio.com/) or VS Code is a popular IDE for Python and several other languages. After installing, see the [getting started](https://code.visualstudio.com/docs/?dv=osx) materials.

[Remote development](https://researchcomputing.princeton.edu/support/knowledge-base/vs-code) is possible on the Research Computing systems. This allows you work with files on a remote system with VS code installed locally on your laptop.

`vim` users should be aware of [VSCodeVim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim) which is an extension that provides `vim` emulation for Visual Studio Code.

## PyCharm

[JetBrains](https://www.jetbrains.com/) provides IDEs for Python, Java, JavaScript, .NET, and more. See [PyCharm](https://www.jetbrains.com/pycharm/) for Python. Get the Professional edition by using your `princeton.edu` email address. With the professional version you can do remote development.

## Recommendations

Princeton Research Computing encourages researchers using the high-performance computing clusters to know one or more tools for simple editing and IDE-like work for software engineering. Here are some good possibilities:

- VS Code and nano/emacs/vim
- PyCharm and nano/emacs/vim
- emacs (fully configured as an IDE)
- vim (fully configured as an IDE)

The general idea is to know a simple text editor and something with IDE features.
