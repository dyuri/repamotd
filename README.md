# repamotd

Display *motd-like* system information.

![repamotd in work](https://raw.githubusercontent.com/dyuri/repamotd/master/repamotd.png)

## Install

Create `$XDG_CONFIG_HOME/repamotd` directory, copy / link the `plugin` directory into it. If `$XDG_CONFIG_HOME` is not set `$HOME/.config` is used.

## Run

```
$ repamotd
```

## Configuration

If you have a `$XDG_CONFIG_HOME/repamotd/env` file, it will be sourced before executing the plugins.

You can override the default colors or the figlet options there.

Example:

```
export COLOR_N="\033[0;38;5;8m"
export COLOR_B="\033[0;38;5;0m"
export COLOR_H1="\033[0;38;5;2m"
export COLOR_H2="\033[1;38;5;10m"
export COLOR_T1="\033[0;38;5;15m"
export COLOR_T2="\033[0;38;5;7m"
export COLOR_E1="\033[0;38;5;1m"
export COLOR_E2="\033[1;38;5;9m"

export FIGLET_OPTS="-d $HOME/figlet -f rebel"
```
