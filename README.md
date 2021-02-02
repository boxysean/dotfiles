## bash

- Install bash-it via brew
- Put this line in `~/.bash_it/themes/bakke/bakke.theme.bash`: ` 20     PS1="\n${cyan}\h: ${reset_color} ${yellow}\w ${red}${scm_prompt_info} ${    purple}${virtualenv_prompt} \n${reset_color}$ "`
- Install fasd and z-autoenv plugins with bash-it

## zsh

- Install [ohmyzsh](https://ohmyz.sh/)
- Change plugins to: `plugins=(git z direnv docker pip pipenv)`
- Change prompt to:
```
export PROMPT='
%(?:%{%}➜ :%{%}➜ ) %{$fg[cyan]%}%c%{$reset_color%} $(git_prompt_info)
$ '
```

## vim

- Install vundle: https://github.com/VundleVim/Vundle.vim#quick-start
- Fix vim: `git config --global core.editor /usr/bin/vim`

## ipython

From https://stackoverflow.com/a/43020072

- Run `ipython profile create`
- Copy `ipython_config.py` to `~/.ipython/profile_default/ipython_config.py`
