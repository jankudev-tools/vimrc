# .vimrc
In the name of Cult of Vi let's embrace [Vim](https://en.wikipedia.org/wiki/Vim_(text_editor)) as the all purpose editor. [Long live Vi, death to Emacs](https://en.wikipedia.org/wiki/Editor_war).

## How it works
It's just some .vimrc configurations that mostly use Vundles for plugin management. It's more a backup of my configurations for various languages support thus creating specific IDEs.

The first thing to do is get Vundle:
```
git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```

Then I create a specific ```.vimrc-language``` file in my HOME folder with the Vundle enabled and with the specific configuration for the IDE.

I usually create a system alias to run Vim with the appropriate .vimrc file into ```.bash_aliases```:
```
alias vim.language='vim ~/.vimrc-language'
```

On the first run of the Vim I need to install the defined plugins:
```
:PluginInstall
```

And there I have a nice IDE.
